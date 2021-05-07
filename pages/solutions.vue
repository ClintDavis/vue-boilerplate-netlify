<template>
  <main>
    <section class="self-center flex flex-col flex-1 items-center justify-center">
      <h1 class="title text-center">Nuxt — Tailwind — Netlify CMS</h1>
      <h2 class="subtitle text-center">Boilerplate</h2>
    </section>

    <section class="mt-8">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam at tellus ac nunc finibus volutpat tincidunt nec magna. Nulla facilisi. Integer lacus sem, gravida eget lobortis et, vehicula fermentum nunc. Fusce ornare eros velit, eu sodales ante elementum id. 
    </section>


    <section class="mt-8">
      <h3>Areas we assist</h3>

      <div class="self-center flex flex-wrap grid grid-cols-3 gap-1 items-center justify-center">
        <div class="" >
          <nuxt-link to="/solution/customer-service">
            <img class="mx-auto -mt-36 md:-mt-36" src="https://picsum.photos/seed/customer/200" />
            <span>Customer Service</span>
          </nuxt-link>
        </div>
        <div class="">
          <nuxt-link to="/solution/debt-collection">
          <img class="mx-auto -mt-36 md:-mt-36" src="https://picsum.photos/seed/debt/200" />
          <span>Debt Collection</span>
          </nuxt-link>
        </div>
        <div class="">
          <nuxt-link to="/solution/finance-agents">
            <img class="mx-auto -mt-36 md:-mt-36" src="https://picsum.photos/seed/finance/200" />
            <span>Finance Agents</span>
          </nuxt-link>
        </div>
        <div class="">
          <nuxt-link to="/solution/accountants">
            <img class="mx-auto -mt-36 md:-mt-36" src="https://picsum.photos/seed/accounting/200" />
            <span>Accounting</span>
          </nuxt-link>
        </div>
        <div class="">
          <nuxt-link to="/solution/bookkeeping">
            <img class="mx-auto -mt-36 md:-mt-36" src="https://picsum.photos/seed/bookkepping/200" />
            <span>Bookeeping</span>
          </nuxt-link>
        </div>
        <div class="">
          <nuxt-link to="/solution/administion">
            <img class="mx-auto -mt-36 md:-mt-36" src="https://picsum.photos/seed/admin/200" />
            <span>Administration</span>
          </nuxt-link>
        </div>
        <div class="">
          <nuxt-link to="/solution/software-dev">
            <img class="mx-auto -mt-36 md:-mt-36" src="https://picsum.photos/seed/software/200" />
            <span>Software Development</span>
          </nuxt-link>
        </div>
        <div class="">
          <nuxt-link to="/solution/it-services">
            <img class="mx-auto -mt-36 md:-mt-36" src="https://picsum.photos/seed/it/200" />
            <span>IT Services</span>
          </nuxt-link>
        </div>
      </div>
    </section>
  </main>
</template>