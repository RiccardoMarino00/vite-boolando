<script>
export default {
    data(){
        return {
            menu: [
                {
                    text: 'Donna',
                    href: '#',
                },
                {
                    text: 'Uomo',
                    href: '#',
                },
                {
                    text: 'Bambino',
                    href: '#',
                },
            ]
        }
    }
}
</script>

<template>
<section class="header">
        <nav>
            <header>
                <div class="container">
                  <div class="row header">
                      <div class="col-header">
                          <span class="genr" v-for="(genere, i) in menu" :key="i">{{ genere.text }}</span>
                      </div>
                      <div class="col-header titolo">
                          <img src="/public/boolean-logo.png" alt="Logo boolean" width="150px">
                      </div>
                      <div class="col-header">
                          Profilo
                      </div>
                  </div>
                </div>
              </header>
        </nav>
    </section>
</template>

<style>

</style>