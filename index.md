---
layout: default
title: myshit.ai
classification: public
---

<!-- Hero -->
<section class="mx-auto max-w-5xl px-6 pt-16 pb-20 md:pt-28 md:pb-28 text-center">
  <p class="font-serif italic text-lg md:text-xl text-muted max-w-2xl mx-auto leading-snug">
    AI tools change. Tech companies change. Fineprints change. <span class="text-ink not-italic font-semibold">But.</span>
  </p>
  <h1 class="mt-5 font-serif font-bold display-tight text-[3rem] sm:text-6xl md:text-7xl lg:text-8xl leading-[1.02] text-ink">
    Your shit should stay&nbsp;yours.
  </h1>
  <p class="mt-8 font-serif text-lg md:text-xl text-ink/70 max-w-xl mx-auto leading-relaxed">
    Stashed on your Mac, used for your good,<br>
    <span class="italic text-ink/55">not for someone else's bottom line.</span>
  </p>

  <details class="mt-10 inline-block text-left group">
    <summary class="inline-flex items-center gap-2 px-6 py-3.5 bg-ink text-cream text-[0.95rem] font-semibold rounded-full cursor-pointer select-none hover:bg-rust transition-colors focus:outline-none focus:ring-2 focus:ring-rust focus:ring-offset-2 focus:ring-offset-cream">
      <span>Sign me up!</span>
      <span class="transition-transform group-open:rotate-90" aria-hidden="true">→</span>
    </summary>
    <div class="reveal-panel mt-5 max-w-md p-5 bg-white border border-ink/10 border-l-[3px] border-l-rust rounded-md">
      <p class="font-serif italic text-ink/70 leading-relaxed text-[0.98rem]">
        Stache is not available to the public yet. Put down an email, he'll buzz you up.
      </p>
      <form id="waitlist-form"
            action="https://docs.google.com/forms/d/e/1FAIpQLSf02IdU0lbL3rWW9IlAJ8y0MmYJFWpyxSG7yL7AzluPR2dnmA/formResponse"
            method="POST" target="waitlist-sink"
            class="mt-4 flex items-stretch gap-2">
        <label for="email" class="sr-only">Email</label>
        <input id="email" type="email" name="entry.1226720376" required placeholder="you@example.com" autocomplete="email"
               class="flex-1 min-w-0 h-12 px-3.5 text-[0.95rem] bg-cream border border-ink/15 rounded-md focus:outline-none focus:border-ink focus:ring-2 focus:ring-ink/10 placeholder:text-muted">
        <input type="text" name="website" tabindex="-1" autocomplete="off" aria-hidden="true"
               style="position:absolute;left:-9999px;width:1px;height:1px;opacity:0">
        <button type="submit" aria-label="Buzz me up"
                class="group relative w-12 h-12 flex-shrink-0 bg-ink hover:bg-rust rounded-md transition-colors focus:outline-none focus:ring-2 focus:ring-rust focus:ring-offset-2 focus:ring-offset-cream">
          <span aria-hidden="true" class="absolute inset-0 flex items-center justify-center text-cream text-xl leading-none transition-opacity duration-200 group-hover:opacity-0">→</span>
          <svg aria-hidden="true" viewBox="0 0 1024 1024" class="absolute inset-0 m-auto h-6 w-auto opacity-0 transition-opacity duration-200 group-hover:opacity-100">
            <path fill="#faf7f2" d="M512 524 C468 406 352 398 288 482 C240 546 168 562 104 520 C118 646 230 728 362 728 C430 728 484 700 512 646 C540 700 594 728 662 728 C794 728 906 646 920 520 C856 562 784 546 736 482 C672 398 556 406 512 524Z"/>
          </svg>
        </button>
      </form>
      <iframe name="waitlist-sink" style="display:none" aria-hidden="true" tabindex="-1"></iframe>
      <p id="waitlist-note" class="mt-3 text-xs text-muted">No spam. One email when he's ready.</p>
      <p id="waitlist-thanks" class="mt-3 text-xs text-rust font-medium hidden">Got it. Stache will buzz when he's ready.</p>
      <script>
        (function () {
          var form = document.getElementById('waitlist-form');
          var sink = document.getElementsByName('waitlist-sink')[0];
          if (!form || !sink) return;
          var submitted = false;
          form.addEventListener('submit', function (e) {
            if (form.website && form.website.value) { e.preventDefault(); return; }
            submitted = true;
          });
          sink.addEventListener('load', function () {
            if (!submitted) return;
            form.style.display = 'none';
            document.getElementById('waitlist-note').classList.add('hidden');
            document.getElementById('waitlist-thanks').classList.remove('hidden');
          });
        })();
      </script>
    </div>
  </details>
</section>

<!-- What's the fuss? -->
<section class="mx-auto max-w-4xl px-6 py-20 md:py-28 border-t border-ink/10">
  <div class="text-center">
    <p class="font-sans text-[0.72rem] font-semibold tracking-[0.18em] uppercase text-rust">
      What's the fuss?
    </p>
    <h2 class="mt-4 font-serif font-semibold text-ink leading-[1.1] display-tight text-[2rem] md:text-5xl">
      To be useful, AI needs specifics.
    </h2>
    <div class="mt-7 font-serif text-lg md:text-xl text-ink/70 max-w-2xl mx-auto leading-relaxed space-y-4">
      <p>
        Imagine a powerful AI system that knows exactly who you are, what you wanna do, why you wanna do it, who you do it with — and everything else that makes you tick… <em class="italic">terribly helpful, or terrifying?</em>
      </p>
      <p>
        The difference is who owns it, and what they decide to do with it.
      </p>
      <p class="text-rust font-semibold">
        We help you build the first one, so you don't have to settle for the second and find out.
      </p>
      <p class="!mt-5">
        <a href="#decay" class="inline-flex items-center gap-1.5 text-rust/80 hover:text-rust text-base font-medium transition-colors group">
          <span class="border-b border-rust/30 group-hover:border-rust">Learn more about platform decay</span>
          <span class="transition-transform group-hover:translate-x-0.5" aria-hidden="true">→</span>
        </a>
      </p>
    </div>
  </div>
</section>

<!-- Comes in the Stache -->
<section class="mx-auto max-w-5xl px-6 py-20 md:py-24 border-t border-ink/10">
  <div class="text-center mb-14 md:mb-16">
    <p class="font-sans text-[0.72rem] font-semibold tracking-[0.18em] uppercase text-rust">Comes in the Stache&trade;</p>
    <h2 class="mt-4 font-serif font-semibold text-ink leading-[1.1] display-tight text-[1.8rem] md:text-4xl">
      Three simple ingredients.
    </h2>
  </div>
  <div class="grid md:grid-cols-3 gap-12 md:gap-10">
    <div class="group cursor-default">
      <img src="/assets/img/stache.svg" alt="" aria-hidden="true" class="h-7 w-auto transition-transform duration-700 ease-out group-hover:rotate-[360deg] motion-reduce:transition-none motion-reduce:group-hover:rotate-0">
      <h3 class="mt-4 font-serif text-xl md:text-2xl font-semibold text-ink leading-tight">
        Stache takes notes.<br>
        <span class="text-ink/55">So you don't have to.</span>
      </h3>
      <p class="mt-3 text-muted leading-relaxed">Docs, meetings, emails, crazy ideas. You throw it, he stashes it where it belongs. No writing, no organizing, no hassle.</p>
    </div>
    <div class="group cursor-default">
      <img src="/assets/img/stache.svg" alt="" aria-hidden="true" class="h-7 w-auto transition-transform duration-700 ease-out group-hover:rotate-[360deg] motion-reduce:transition-none motion-reduce:group-hover:rotate-0">
      <h3 class="mt-4 font-serif text-xl md:text-2xl font-semibold text-ink leading-tight">
        Stache briefs AI tools.<br>
        <span class="text-ink/55">So you don't have to.</span>
      </h3>
      <p class="mt-3 text-muted leading-relaxed">No more generic AI slop. ChatGPT, Claude, or whatever's next. He shares just what they need to know on a need-to-know basis.</p>
    </div>
    <div class="group cursor-default md:pl-6 md:border-l md:border-rust/30">
      <img src="/assets/img/stache.svg" alt="" aria-hidden="true" class="h-7 w-auto transition-transform duration-700 ease-out group-hover:rotate-[360deg] motion-reduce:transition-none motion-reduce:group-hover:rotate-0">
      <h3 class="mt-4 font-serif text-xl md:text-2xl font-semibold text-ink leading-tight">
        Stache doesn't creep.<br>
        <span class="text-ink/55">And shuts out others too.</span>
      </h3>
      <p class="mt-3 text-muted leading-relaxed">
        <span class="text-ink">All your data sits on your Mac. Plain and simple.</span> Read it, edit it, take it where you need it. It's your shit, not ours.
      </p>
    </div>
  </div>
</section>

<!-- What keeps Stache up at night -->
<section id="decay" class="mx-auto max-w-5xl px-6 py-20 md:py-28 border-t border-ink/10 scroll-mt-8">
  <div class="text-center mb-12 md:mb-16">
    <p class="font-sans text-[0.72rem] font-semibold tracking-[0.18em] uppercase text-rust">
      What keeps Stache up at night
    </p>
    <h2 class="mt-4 font-serif font-semibold text-ink leading-[1.1] display-tight text-[1.8rem] md:text-4xl max-w-3xl mx-auto">
      How things go bad when your data's out there.
    </h2>
  </div>

  <div class="grid md:grid-cols-3 gap-10 md:gap-10 mb-14 md:mb-16">
    <div>
      <p class="font-sans text-[0.65rem] font-semibold tracking-[0.18em] uppercase text-rust mb-2">Lock-in</p>
      <h3 class="font-serif text-xl md:text-2xl font-semibold text-ink leading-tight">You get hooked,<br>and the deal turns sour.</h3>
      <p class="mt-4 font-serif text-base md:text-lg text-ink/75 leading-relaxed">
        You sign on for free, fast, frictionless. You build on it. It becomes <em>the</em> place. Then, slowly, the deal turns. Charges appear. Defaults shift. Reach narrows. The picture you helped build no longer answers to you. The pattern even has a name now: <em>enshittification</em>, the American Dialect Society's 2023 Word of the Year. Facebook, Amazon, Uber &mdash; pick your favorite.
      </p>
      <p class="mt-5 text-[0.82rem] text-ink/70 leading-relaxed">
        Read more about enshittification (platform decay):
        <a href="https://en.wikipedia.org/wiki/Enshittification" class="underline underline-offset-2 decoration-1 hover:text-rust hover:decoration-2" target="_blank" rel="noopener">Wikipedia</a>
      </p>
    </div>
    <div>
      <p class="font-sans text-[0.65rem] font-semibold tracking-[0.18em] uppercase text-rust mb-2">Misuse</p>
      <h3 class="font-serif text-xl md:text-2xl font-semibold text-ink leading-tight">Hand it over once,<br>and it's out of your hands.</h3>
      <p class="mt-4 font-serif text-base md:text-lg text-ink/75 leading-relaxed">
        Sometimes there was no deal at all. Your face from a friend's tag, in a face-rec database. Your voice memo, overheard by a contractor. Your neighborhood ping, in a court warrant. <span class="text-ink">Things you'd have said no to, if anyone had bothered to ask.</span>
      </p>
      <div class="mt-5">
        <p class="text-rust font-semibold uppercase tracking-[0.18em] text-[0.65rem] mb-2">Read past examples</p>
        <ul class="text-[0.82rem] text-ink/70 leading-relaxed space-y-1">
          <li>
            Your face mined:
            <a href="https://www.nytimes.com/interactive/2021/03/18/magazine/facial-recognition-clearview-ai.html" class="underline underline-offset-2 decoration-1 hover:text-rust hover:decoration-2" target="_blank" rel="noopener">NY Times</a>
            <span class="text-ink/30 mx-1">&middot;</span>
            <a href="https://en.wikipedia.org/wiki/Clearview_AI" class="underline underline-offset-2 decoration-1 hover:text-rust hover:decoration-2" target="_blank" rel="noopener">Wikipedia</a>
          </li>
          <li>
            Your voice overheard:
            <a href="https://www.theguardian.com/technology/2019/jul/26/apple-contractors-regularly-hear-confidential-details-on-siri-recordings" class="underline underline-offset-2 decoration-1 hover:text-rust hover:decoration-2" target="_blank" rel="noopener">The Guardian</a>
            <span class="text-ink/30 mx-1">&middot;</span>
            <a href="https://www.reuters.com/legal/apple-pay-95-million-settle-siri-privacy-lawsuit-2025-01-02/" class="underline underline-offset-2 decoration-1 hover:text-rust hover:decoration-2" target="_blank" rel="noopener">Reuters</a>
          </li>
          <li>
            Your location tracked:
            <a href="https://www.nytimes.com/2026/01/16/us/politics/supreme-court-warrants-location-data.html" class="underline underline-offset-2 decoration-1 hover:text-rust hover:decoration-2" target="_blank" rel="noopener">NY Times</a>
          </li>
        </ul>
      </div>
    </div>
    <div>
      <p class="font-sans text-[0.65rem] font-semibold tracking-[0.18em] uppercase text-rust mb-2">Drift</p>
      <h3 class="font-serif text-xl md:text-2xl font-semibold text-ink leading-tight">The company goes down, your data goes up for sale.</h3>
      <p class="mt-4 font-serif text-base md:text-lg text-ink/75 leading-relaxed">
        When a company goes bankrupt, you'd lose your data, if you're lucky. If not, your data becomes a liquid asset, sold for scraps. Think DNA from fifteen million people, sold for scraps.
      </p>
      <p class="mt-5 text-[0.82rem] text-ink/70 leading-relaxed">
        Read more about 23andMe bankruptcy:
        <a href="https://www.nytimes.com/2025/06/10/business/23andme-data-lawsuit.html" class="underline underline-offset-2 decoration-1 hover:text-rust hover:decoration-2" target="_blank" rel="noopener">NY Times</a>
        <span class="text-ink/30 mx-1">&middot;</span>
        <a href="https://en.wikipedia.org/wiki/23andMe" class="underline underline-offset-2 decoration-1 hover:text-rust hover:decoration-2" target="_blank" rel="noopener">Wikipedia</a>
      </p>
    </div>
  </div>

  <div class="font-serif text-base md:text-lg text-ink/75 max-w-2xl mx-auto leading-relaxed text-center">
    <p>
      Stache can't fix it all. But he can help you do one thing &mdash; refuse to be a source of any of them. When the picture lives on your own computer, in files you control: the deal can't change on you. The company can't disappear with your stuff. Nobody at HQ has anyone's data to get clever with. <span class="text-ink">Stache wants to get ahead of that.</span>
    </p>
  </div>
</section>
