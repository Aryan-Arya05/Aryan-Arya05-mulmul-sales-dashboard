# Mulmul Sales · Replenishment · Production dashboard

Internal dashboard for Shop Mulmul: sales by launch and product, replenishment, production, inwards, stock aging and an Ask box.

- **App:** `index.html`, served by GitHub Pages at https://sales.mulmul.co/. It holds no data.
- **Sign-in:** Mulmul Threads accounts. Access is given in Threads under Admin, People & access ("Sales & Replenishment").
- **Data:** the `mulmul-stock-lookup` Supabase project. Every request goes through its `dash` edge function, which checks the
  person's Threads access first. The function, the database views and the sync jobs live in the
  [mulmul-stock-lookup](https://github.com/Aryan-Arya05/mulmul-stock-lookup) repo (`supabase/functions/dash`, `scripts/`, `sales/README.md`).

Never commit data files to this repo. It is public; data stays in the database behind sign-in.
