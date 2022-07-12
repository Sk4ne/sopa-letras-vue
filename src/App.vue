<template>
  <div id="app">
    <div class="container" id="main">
    <div class="row">
      <div class="mt-4 col-md-12">
         <h1 class="text-center">Palabras a encontrar</h1>
         <ul>
           <li id="CAMELLO">CAMELLO</li>
           <li id="TIGRE">TIGRE</li>
           <li id="CABALLO">CABALLO</li>
           <li id="VACA">VACA</li>
           <li id="NU">ÑU</li>
         </ul>
      </div>
    </div>
    <!-- second row -->
    <div class="row">
      <div class="col-md-3">
        <table class="table table-bordered">
          <thead>
            <tr>
              <th><img :src="tigger" class='w-25 img-fluid' alt=""></th>
            </tr>
            <tr>
              <th><img :src="camel" class='w-25 img-fluid' alt=""></th>
            </tr>
            <tr>
              <th><img :src="horse" class='w-25 img-fluid' alt=""></th>
            </tr>
          </thead>
        </table>
      </div>
      <div class="col-md-6">
        <table class="table table-bordered">
          <thead>
            <tr>
              <th class="text-center">S</th>
              <th class="text-center">X</th>
              <th class="text-center">O</th>
              <th class="text-center">Ñ</th>
              <th class="text-center" ref="tigger-1" @click="tig1()">T</th>
              <th class="text-center">U</th>
              <th class="text-center">Y</th>
              <th class="text-center">Z</th>
              <th class="text-center" ref="vaca-1" @click="vac1()">V</th>
              <th class="text-center" ref='word-1' @click="c1()">C</th>
            </tr>
            <tr> 
              <th class="text-center">C</th>
              <th class="text-center">Y</th>
              <th class="text-center" ref="horse-1" @click="hor1()">O</th>
              <th class="text-center">B</th>
              <th class="text-center" ref="tigger-2" @click="tig2()">I</th>
              <th class="text-center">U</th>
              <th class="text-center">A</th>
              <th class="text-center">Z</th>
              <th class="text-center word-2 vaca-2" @click="c2(),vac2()" >A</th>
              <th class="text-center">B</th>
            </tr>
            <tr>
              <th class="text-center">K</th>
              <th class="text-center">Ñ</th>
              <th class="text-center" ref="horse-2" @click="hor2()">L</th>
              <th class="text-center">A</th>
              <th class="text-center" ref="tigger-3" @click="tig3()">G</th>
              <th class="text-center">R</th>
              <th class="text-center">V</th>
              <th class="text-center" ref="word-3" @click="c3()">M</th>
              <th class="text-center" ref="vaca-3" @click="vac3()">C</th>
              <th class="text-center">B</th>
            </tr>
            <tr>
              <th class="text-center">V</th>
              <th class="text-center">M</th>
              <th class="text-center" ref="horse-3" @click="hor3()">L</th>
              <th class="text-center">L</th>
              <th class="text-center" ref="tigger-4" @click="tig4()">R</th>
              <th class="text-center">T</th>
              <th class="text-center" ref="word-4" @click="c4()">E</th>
              <th class="text-center">Z</th>
              <th class="text-center" ref="vaca-4" @click="vac4()">A</th>
              <th class="text-center" ref="nu-1" @click="nu1()">Ñ</th>
            </tr>
            <tr>
              <th class="text-center">U</th>
              <th class="text-center">M</th>
              <th class="text-center" ref="horse-4" @click="hor4()">A</th>
              <th class="text-center">A</th>
              <th class="text-center" ref="tigger-5" @click="tig5()">E</th>
              <th class="text-center" ref="word-5" @click="c5()">L</th>
              <th class="text-center">L</th>
              <th class="text-center">Z</th>
              <th class="text-center">T</th>
              <th class="text-center" ref="nu-2" @click="nu2()">U</th>
            </tr>
            <tr>
              <th class="text-center">T</th>
              <th class="text-center">A</th>
              <th class="text-center" ref="horse-5" @click="hor5()">B</th>
              <th class="text-center">K</th>
              <th class="text-center" ref="word-6" @click="c6()">L</th>
              <th class="text-center">U</th>
              <th class="text-center">X</th>
              <th class="text-center">E</th>
              <th class="text-center">K</th>
              <th class="text-center">W</th>
            </tr>
            <tr>
              <th class="text-center">R</th>
              <th class="text-center">X</th>
              <th class="text-center" ref="horse-6" @click="hor6()">A</th>
              <th class="text-center" ref="word-7" @click="c7()">O</th>
              <th class="text-center">T</th>
              <th class="text-center">U</th>
              <th class="text-center">O</th>
              <th class="text-center">R</th>
              <th class="text-center">G</th>
              <th class="text-center">U</th>
            </tr>
            <tr>
              <th class="text-center">P</th>
              <th class="text-center">X</th>
              <th class="text-center" ref="horse-7" @click="hor7()">C</th>
              <th class="text-center">Ñ</th>
              <th class="text-center">T</th>
              <th class="text-center">U</th>
              <th class="text-center">Q</th>
              <th class="text-center">Z</th>
              <th class="text-center">L</th>
              <th class="text-center">I</th>
            </tr>
          </thead>
        </table>
      </div>
      <div class="col-md-3">
        <table class="table table-bordered">
          <thead>
            <tr>
              <th><img :src="cow" class='w-25 img-fluid' alt=""></th>
            </tr>
            <tr>
              <th><img :src="nu" class='w-25 img-fluid' alt=""></th>
            </tr>
            <tr>
              <th><img :src="tigger" class='w-25 img-fluid' alt=""></th>
            </tr>
          </thead>
        </table>
      </div>
    </div>

    <div class="row">
      <div class="offset-md-4 col-md-4">
        <button class="btn btn-secondary btn-block" @click="test()" >Finalizar</button>
        <button class="btn btn-secondary btn-block" @click="reloadPage()" >Reiniciar</button>
      </div>
    </div>
    <br><br><br><br>
  </div>
  </div>
</template>

<script>
import $ from "jquery";
export default {
  name: 'App',
  components: {
  },
  data(){
    return{
      win:0,
      letra1:null,
      l1:null,l2:null,l3:null,l4:null,l5:null,l6:null,l7:null,
      h1:null,h2:null,h3:null,h4:null,h5:null,h6:null,h7:null,
      t1:null,t2:null,t3:null,t4:null,t5:null,
      v1:null,v2:null,v3:null,v4:null,
      lA1:null,lA2:null,
      tigger: 'https://res.cloudinary.com/dqhme1rod/image/upload/v1657551093/myimages/s-l/anlfyfxmlfvp9iibqmdn.png',
      cow:'https://res.cloudinary.com/dqhme1rod/image/upload/v1657591959/myimages/s-l/fx5m1gdalteos85o0pop.png',
      horse: 'https://res.cloudinary.com/dqhme1rod/image/upload/v1657591959/myimages/s-l/awd59gnxd2eah9na7szb.png',
      camel:'https://res.cloudinary.com/dqhme1rod/image/upload/v1657591959/myimages/s-l/i6l0tdkkzqm9ocxfzxjk.png',
      nu:'https://res.cloudinary.com/dqhme1rod/image/upload/v1657591959/myimages/s-l/vxp4uwy76wyjqqvftmfc.png'
    }
  },
  methods: {
    reloadPage() {
      window.location.reload();
    },
    // WORD CAMELLO
    c1(){
      // this.l1 = document.getElementById('word-1').style.backgroundColor = 'darkcyan';
      this.l1 = this.$refs['word-1'].style.backgroundColor = 'darkcyan';
    },
    c2(){
      this.l2 = document.querySelector('.word-2').style.backgroundColor = 'darkcyan';
    },
    c3(){
      this.l3 = this.$refs['word-3'].style.backgroundColor = 'darkcyan';
    },
    c4(){
      this.l4 = this.$refs['word-4'].style.backgroundColor = 'darkcyan';
    },
    c5(){
      this.l5 = this.$refs['word-5'].style.backgroundColor = 'darkcyan';
    },
    c6(){
      this.l6 = this.$refs['word-6'].style.backgroundColor = 'darkcyan';
    },
    c7(){
      this.l7 = this.$refs['word-7'].style.backgroundColor = 'darkcyan';
    },
    /* WORD CABALLO */
    hor1(){
      this.h1 = this.$refs['horse-1'].style.backgroundColor = 'darkcyan';
    },
    hor2(){
      this.h2 = this.$refs['horse-2'].style.backgroundColor = 'darkcyan';
    },
    hor3(){
      this.h3 = this.$refs['horse-3'].style.backgroundColor = 'darkcyan';
    },
    hor4(){
      this.h4 = this.$refs['horse-4'].style.backgroundColor = 'darkcyan';
    },
    hor5(){
      this.h5 = this.$refs['horse-5'].style.backgroundColor = 'darkcyan';
    },
    hor6(){
      this.h6 = this.$refs['horse-6'].style.backgroundColor = 'darkcyan';
    },
    hor7(){
      this.h7 = this.$refs['horse-7'].style.backgroundColor = 'darkcyan';
    },
    /* word tigre */
    /* TIGRE */
    tig1(){
      this.t1 = this.$refs['tigger-1'].style.backgroundColor = 'darkcyan';
    },
    tig2(){
      this.t2 = this.$refs['tigger-2'].style.backgroundColor = 'darkcyan';
    },
    tig3(){
      this.t3 = this.$refs['tigger-3'].style.backgroundColor = 'darkcyan';
    },
    tig4(){
      this.t4 = this.$refs['tigger-4'].style.backgroundColor = 'darkcyan';
    },
    tig5(){
      this.t5 = this.$refs['tigger-5'].style.backgroundColor = 'darkcyan';
    },
    /* word vaca */
    /* VACA */
    vac1(){
      this.v1 = this.$refs['vaca-1'].style.backgroundColor = 'darkcyan';
    },
    vac2(){
      this.v2 = document.querySelector('.vaca-2').style.backgroundColor = 'darkcyan';
    },
    vac3(){
      this.v3 = this.$refs['vaca-3'].style.backgroundColor = 'darkcyan';
    },
    vac4(){
      this.v4 = this.$refs['vaca-4'].style.backgroundColor = 'darkcyan';
    },
    /* word ñu */
    nu1(){
      this.lA1 = this.$refs['nu-1'].style.backgroundColor = 'darkcyan';
    },
    nu2(){
      this.lA2 = this.$refs['nu-2'].style.backgroundColor = 'darkcyan';
    },
    test(){
      if(this.l1 == 'darkcyan' && this.l2 == 'darkcyan' && this.l3 == 'darkcyan' && this.l4 == 'darkcyan' && this.l5 == 'darkcyan' && this.l6 == 'darkcyan' && this.l7 == 'darkcyan'){
       $(document.getElementById('CAMELLO')).css('text-decoration', 'line-through');
       this.win+=1;
      }
      if(this.h1 == 'darkcyan' && this.h2 == 'darkcyan' && this.h3 == 'darkcyan' && this.h4 == 'darkcyan' && this.h5 == 'darkcyan' && this.h6 == 'darkcyan' && this.h7 == 'darkcyan'){
        $(document.getElementById('CABALLO')).css('text-decoration', 'line-through');
        this.win+=1;
      }
      if(this.t1 == 'darkcyan' && this.t2 == 'darkcyan' && this.t3 == 'darkcyan' && this.t4 == 'darkcyan' && this.t5 == 'darkcyan'){
        $(document.getElementById('TIGRE')).css('text-decoration', 'line-through');
        this.win+=1;
      }
      if(this.v1 == 'darkcyan' && this.v2 == 'darkcyan' && this.v3 == 'darkcyan' && this.v4 == 'darkcyan'){
        $(document.getElementById('VACA')).css('text-decoration', 'line-through');
        this.win+=1;
      }
      if(this.lA1 == 'darkcyan' && this.lA2 == 'darkcyan'){
        $(document.getElementById('NU')).css('text-decoration', 'line-through');
        this.win+=1;
      }
      if(this.win === 5){
        console.log('PERFECTO, GANASTE !!! ');
        alert('PERFECTO, GANASTE !!!');
      }
      else{
        console.log('PERDISTE VUELVE A INTENTARLO :)');
        alert('PERDISTE INTENTALO DE NUEVO.'); 
      }
    }
  }
}
</script>
