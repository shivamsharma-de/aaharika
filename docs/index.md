<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta content="width=device-width, initial-scale=1.0" name="viewport" />
    <title>Gabbu Cooks</title>
    <script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
    <link
      href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=Instrument+Serif:italic@0;1&display=swap"
      rel="stylesheet"
    />
    <link
      href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&display=swap"
      rel="stylesheet"
    />
    <style type="text/tailwindcss">
      :root {
        --bg-canvas: #fdfaf6;
        --accent-clay: #d97757;
        --accent-sage: #8b9d83;
        --accent-sand: #e8e1d3;
        --text-main: #3d3a35;
      }
      body {
        font-family: "Plus Jakarta Sans", sans-serif;
        background-color: var(--bg-canvas);
        color: var(--text-main);
      }
      .serif-italic {
        font-family: "Instrument Serif", serif;
      }
      .bento-card {
        @apply bg-white border border-[#e8e1d3] rounded-[2.5rem] transition-all duration-300 hover:shadow-xl hover:shadow-[#8b9d83]/10;
      }
      .scrapbook-label {
        @apply absolute -top-3 -left-2 bg-white px-4 py-1 rounded-full border border-[#e8e1d3] text-[10px] font-bold uppercase tracking-widest shadow-sm;
      }
      .sketch-underline {
        background-image: linear-gradient(120deg, #d97757 0%, #d97757 100%);
        background-repeat: no-repeat;
        background-size: 100% 0.2em;
        background-position: 0 88%;
      }
    </style>
    <script id="tailwind-config">
      tailwind.config = {
        theme: {
          extend: {
            colors: {
              clay: "#d97757",
              sage: "#8b9d83",
              sand: "#e8e1d3",
              canvas: "#fdfaf6",
              ink: "#3d3a35",
            },
          },
        },
      };
    </script>
  </head>
  <body class="p-4 md:p-8 lg:p-12 selection:bg-clay/20">
    <div class="max-w-[1400px] mx-auto">
      <header class="flex justify-between items-center mb-16 px-4">
        <div class="flex items-center gap-4">
          <div
            class="size-12 rounded-full bg-clay flex items-center justify-center text-white font-bold text-xl"
          >
            G
          </div>
          <div>
            <h1 class="font-bold text-lg leading-none">Gabbu Cooks</h1>
            <p class="text-xs text-sage font-medium italic">
              Food, craft, and learning
            </p>
          </div>
        </div>
        <nav class="hidden md:flex gap-8 text-sm font-semibold text-ink/60">
          <a class="hover:text-clay transition-colors" href="./aaharika/">Aaharika</a>
          <a class="hover:text-clay transition-colors" href="#">Woodworking</a>
          <a class="hover:text-clay transition-colors" href="#">Articles</a>
          <a class="hover:text-clay transition-colors" href="#">Career</a>
        </nav>
        <a
          class="bg-ink text-canvas px-6 py-3 rounded-full text-sm font-bold hover:scale-105 transition-transform active:scale-95"
          href="./aaharika/"
        >
          Explore Aaharika
        </a>
      </header>
      <main class="grid grid-cols-1 md:grid-cols-12 gap-6 items-start">
        <section
          class="md:col-span-8 bento-card p-10 md:p-16 relative overflow-hidden flex flex-col justify-center min-h-[500px]"
        >
          <div class="relative z-10 max-w-2xl">
            <span
              class="text-clay font-bold text-sm mb-4 block tracking-widest uppercase"
              >Multi-project hub</span
            >
            <h2
              class="text-5xl md:text-7xl font-extrabold leading-[1.1] mb-8 tracking-tight"
            >
              I build products, <span class="serif-italic text-clay font-normal lowercase">cook</span>
              food, &amp; chase
              <span class="serif-italic text-clay font-normal lowercase">craft</span>.
            </h2>
            <p class="text-xl text-ink/60 leading-relaxed max-w-lg">
              A casual corner of the web where recipes, woodworking, articles,
              and career learning live together.
            </p>
          </div>
          <div class="absolute top-10 right-10 rotate-12 opacity-10">
            <span class="material-symbols-outlined text-[120px]">brush</span>
          </div>
        </section>
        <div class="md:col-span-4 grid grid-cols-2 gap-4 h-full">
          <div
            class="bento-card bg-sand/30 flex items-center justify-center aspect-square md:aspect-auto hover:-rotate-3 transition-transform"
          >
            <span class="material-symbols-outlined text-clay text-5xl"
              >restaurant</span
            >
          </div>
          <div
            class="bento-card bg-sage/10 flex items-center justify-center aspect-square md:aspect-auto hover:rotate-3 transition-transform"
          >
            <span class="material-symbols-outlined text-sage text-5xl"
              >carpenter</span
            >
          </div>
          <div
            class="bento-card bg-clay/10 flex items-center justify-center aspect-square md:aspect-auto hover:rotate-2 transition-transform"
          >
            <span class="material-symbols-outlined text-clay text-5xl"
              >auto_stories</span
            >
          </div>
          <div
            class="bento-card bg-sand/30 flex items-center justify-center aspect-square md:aspect-auto hover:-rotate-2 transition-transform"
          >
            <span class="material-symbols-outlined text-ink text-5xl"
              >explore</span
            >
          </div>
        </div>
        <section class="md:col-span-5 bento-card p-8 group overflow-hidden">
          <div class="relative">
            <div class="flex items-center justify-between mb-8">
              <div
                class="size-14 rounded-2xl bg-sand/50 flex items-center justify-center text-ink"
              >
                <span class="material-symbols-outlined">restaurant</span>
              </div>
              <span class="text-[10px] font-black uppercase tracking-widest text-ink/30"
                >01 — Aaharika</span
              >
            </div>
            <h3 class="text-3xl font-bold mb-4">Aaharika Cookbook</h3>
            <p class="text-ink/60 text-sm mb-6 leading-relaxed">
              Vegetarian and vegan recipes for immigrants in Europe, organized by
              prep time and meal size.
            </p>
            <div class="flex flex-wrap gap-2">
              <span class="px-3 py-1 bg-sand/40 rounded-full text-[10px] font-bold text-ink/70"
                >QUICK MEALS</span
              >
              <span class="px-3 py-1 bg-sand/40 rounded-full text-[10px] font-bold text-ink/70"
                >MEAL PREP</span
              >
              <span class="px-3 py-1 bg-sand/40 rounded-full text-[10px] font-bold text-ink/70"
                >DESSERTS</span
              >
            </div>
          </div>
        </section>
        <section
          class="md:col-span-7 bento-card p-0 overflow-hidden group flex flex-col md:flex-row min-h-[300px]"
        >
          <div
            class="w-full md:w-1/2 h-48 md:h-full bg-cover bg-center grayscale group-hover:grayscale-0 transition-all duration-700"
            style="
              background-image: url('https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=900&q=80');
            "
          ></div>
          <div class="w-full md:w-1/2 p-10 flex flex-col justify-center">
            <span class="text-clay font-bold text-[10px] tracking-[0.2em] mb-4 uppercase"
              >Latest from Kitchen</span
            >
            <h3 class="text-4xl font-bold mb-4 serif-italic">Aaharika Guide.</h3>
            <p class="text-ink/60 text-sm mb-6">
              Explore the cookbook hub and start with the foundations.
            </p>
            <a
              class="text-clay font-bold text-sm flex items-center gap-2 group/link"
              href="./aaharika/"
            >
              Read Cookbook
              <span
                class="material-symbols-outlined transition-transform group-hover/link:translate-x-1"
                >arrow_forward</span
              >
            </a>
          </div>
        </section>
        <section class="md:col-span-4 bento-card p-8 bg-sage/5 relative overflow-hidden">
          <div class="scrapbook-label">In Progress</div>
          <div class="mt-4">
            <h3 class="text-3xl font-bold mb-2">Next Projects</h3>
            <p class="text-ink/60 text-sm mb-8">
              Woodworking builds, learning notes, and long-form essays will live
              here next.
            </p>
            <div class="flex items-end gap-2 mb-2">
              <span class="text-5xl font-black text-sage">4</span>
              <span class="text-xs font-bold text-ink/40 pb-2">QUEUES</span>
            </div>
            <div class="w-full bg-sage/20 h-2 rounded-full overflow-hidden">
              <div class="bg-sage h-full w-[45%]"></div>
            </div>
          </div>
        </section>
        <section
          class="md:col-span-4 bento-card p-8 bg-clay/5 flex flex-col justify-between min-h-[250px] relative"
        >
          <span class="material-symbols-outlined text-clay/20 text-6xl absolute top-4 right-4"
            >format_quote</span
          >
          <p class="text-2xl font-bold text-ink leading-snug serif-italic italic mt-8">
            "Cooking is the shortest route between memory and joy."
          </p>
          <div class="flex items-center gap-3">
            <div class="size-8 rounded-full bg-clay/20 flex items-center justify-center">
              <span class="material-symbols-outlined text-clay text-sm">edit</span>
            </div>
            <span class="text-[10px] font-bold uppercase tracking-widest text-ink/40"
              >Gabbu Notes — 2024</span
            >
          </div>
        </section>
        <section class="md:col-span-4 bento-card overflow-hidden h-full min-h-[250px]">
          <div class="grid grid-cols-2 h-full">
            <div
              class="bg-cover bg-center h-full grayscale hover:grayscale-0 transition-all"
              style="
                background-image: url('https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=600&q=80');
              "
            ></div>
            <div
              class="bg-cover bg-center h-full grayscale hover:grayscale-0 transition-all border-l border-sand/30"
              style="
                background-image: url('https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?auto=format&fit=crop&w=600&q=80');
              "
            ></div>
          </div>
        </section>
      </main>
      <footer
        class="mt-20 pt-16 border-t border-sand flex flex-col md:flex-row justify-between items-center gap-8 pb-12"
      >
        <div class="text-center md:text-left">
          <p class="text-2xl font-bold mb-2">
            Let's grow something <span class="sketch-underline">together</span>.
          </p>
          <p class="text-ink/40 text-sm">
            Email for collaborations or recipes you'd like featured.
          </p>
        </div>
        <div class="flex gap-4">
          <a
            class="size-12 rounded-full border border-sand flex items-center justify-center hover:bg-clay hover:text-white transition-all"
            href="mailto:hello@gabbucooks.com"
          >
            <span class="material-symbols-outlined">alternate_email</span>
          </a>
          <a
            class="size-12 rounded-full border border-sand flex items-center justify-center hover:bg-sage hover:text-white transition-all"
            href="./aaharika/"
          >
            <span class="material-symbols-outlined">menu_book</span>
          </a>
          <a
            class="px-8 h-12 rounded-full bg-ink text-canvas flex items-center justify-center font-bold text-sm"
            href="./aaharika/"
          >
            View Cookbook
          </a>
        </div>
      </footer>
    </div>
  </body>
</html>
