<script>
export default {
  data(){
    return{
      message: 'ciao'
    }
  }
}
</script>

<template>
 <body class="debug">
    <section class="header">
        <nav>
            <header>
                <div class="container">
                  <div class="row header">
                      <div class="col-header">
                          <span>Donna</span>
                          <span>Uomo</span>
                          <span>Bambini</span>
                      </div>
                      <div class="col-header">
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
    
    

    <main>
        <section class="main">
            <div class="container">
                <div class="row">
                    <div class="col-4">
                        <div class="card">
                            <div class="card-header">
                                <img src="/public/1.webp" alt="">
                                <span class="sconto">-50%</span>
                                <span class="eco-friendly">Sostenibilità</span>
                                <span class="cuore">&hearts;</span>
                                <div class="overlay relaxed"></div>
                            </div>
                            <div class="card-body">
                                <p class="littlegray">Levi's</p>
                                <h3>Relaxed fit tee unisex</h3>
                                <p><span class="prize-red">14,99&euro;  </span><span class="text-line">29,99&euro;</span></p>
                            </div>
                        </div>
                    </div>
    
                    <div class="col-4">
                        <div class="card">
                            <div class="card-header">
                                <img src="/public/2.webp" alt="">
                                <span class="sconto">-30%</span>
                                <span class="cuore">&hearts;</span>
                                <div class="overlay guess"></div>
                            </div>
                            <div class="card-body">
                                <p class="littlegray">Guess</p>
                                <h3>Roses Tee</h3>
                                <p><span class="prize-red">14,99&euro;  </span><span class="text-line">29,99&euro;</span></p>
                            </div>
                        </div>
                    </div>
    
                    <div class="col-4">
                        <div class="card">
                            <div class="card-header">
                                <img src="/public/3.webp" alt="">
                                <span class="sconto">-30%</span>
                                <span class="cuore">&hearts;</span>
                                <div class="overlay zucchero"></div>
                            </div>
                            <div class="card-body">
                                <p class="littlegray">Come Zucchero Filato</p>
                                <h3>VOglia di colori pastello</h3>
                                <p><span class="prize-red">14,99&euro;  </span><span class="text-line">29,99&euro;</span></p>
                            </div>
                        </div>
                    </div>
    
                    <div class="col-4">
                        <div class="card">
                            <div class="card-header">
                                <img src="/public/4.webp" alt="">
                                <span class="sconto">-50%</span>
                                <span class="eco-friendly">Sostenibilità</span>
                                <span class="cuore">&hearts;</span>
                                <div class="overlay levis"></div>
                            </div>
                            <div class="card-body">
                                <p class="littlegray">Levi's</p>
                                <h3>Tee unisex</h3>
                                <p><span class="prize-red">14,99&euro;  </span><span class="text-line">29,99&euro;</span></p>
                            </div>
                        </div>
                    </div>
    
                    <div class="col-4">
                        <div class="card">
                            <div class="card-header">
                                <img src="/public/5.webp" alt="">
                                <span class="cuore">&hearts;</span>
                                <div class="overlay maya"></div>
                            </div>
                            <div class="card-body">
                                <p class="littlegray">Maya Deluxe</p>
                                <h3>Stripe bodice</h3>
                                <p><span class="prize-red">14,99&euro;  </span><span class="text-line">29,99&euro;</span></p>
                            </div>
                        </div>
                    </div>
    
                    <div class="col-4">
                        <div class="card">
                            <div class="card-header">
                                <img src="/public/6.webp" alt="">
                                <span class="eco-friendly-woman">Sostenibilità</span>
                                <span class="cuore">&hearts;</span>
                                <div class="overlay espirit"></div>
                            </div>
                            <div class="card-body">
                                <p class="littlegray">Esprit</p>
                                <h3>Maglione-Black</h3>
                                <p><span class="prize-red">14,99&euro;  </span><span class="text-line">29,99&euro;</span></p>   
                            </div>
                        </div>
                    </div>
    
                   
                </div>
            </div>

        </section>
        
    </main>

    <footer>
        <section class="footer">
            <div class="container">
                <div class="row footer">
                    <div class="col">
                        <h3>Boolando s.r.l.</h3>
                        <a href="#" ><span>Informazioni legali</span></a>
                        <a href="#" class="info"><span>Informazioni sulla privacy</span></a>
                        <a href="#" class="info"><span>Diritto di recesso</span></a>
                    </div>
                    <div class="col">                
                           <a href="#"><img src="/public/facebook (1).png" alt="" class="social"></a>
                            <a href="#"><img src="/public/instagram (1).png" alt="" class="social"></a>
                            <a href="#"><img src="/public/twitter (1).png" alt="" class="social"></a>
                            <a href="#"><img src="/public/youtube (1).png" alt="" class="social"></a>    
                    </div>              
                </div>
            </div>

        </section>
        
    </footer>
    
</body>
</template>

<style lang="scss">
@use './style/general';

</style>
