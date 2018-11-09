<template>
  <div id="app">
    <div>
      <input v-model="doc.tipo" type="text" placeholder="Tipo doc N°/Ano">
      <br>
      <form @submit.prevent="itens.push(item); item = {}">
        <input v-model="item.patrimonio" type="text" placeholder="patrimonio">
        <input v-model="item.descricao" type="text" placeholder="descricao">
        <input v-model="item.estado" type="text" placeholder="estado">
        <button type="submit">Adicionar</button>
      </form>
    </div>
    <div>
        <p class="c3"><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 63.00px; height: 57.00px;"><img alt="" src="./images/image2.png" style="width: 63.00px; height: 57.00px; margin-left: -0.00px; margin-top: -0.00px; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px);" title=""></span></p>
        <p class="c3 c4"><span class="c11"></span></p>
        <p class="c3"><span class="c8">Universidade Federal do Rio Grande do Norte</span></p>
        <p class="c3"><span class="c8">ESCOLA AGR&Iacute;COLA DE JUNDIA&Iacute;</span></p>
        <p class="c3 c4"><span class="c26"></span></p>
        <a id="t.b3078c2d13ec230ce3373a6158b164f471d4c106"></a>
        <a id="t.1"></a>
        <table class="c25">
            <tbody>
                <tr class="c13">
                    <td class="c17" colspan="1" rowspan="1">
                        <p class="c18"><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 67.33px; height: 33.20px;"><img alt="logo_eaj" src="./images/image1.jpg" style="width: 67.33px; height: 33.20px; margin-left: -0.00px; margin-top: -0.00px; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px);" title=""></span></p>
                    </td>
                    <td class="c17" colspan="1" rowspan="1">
                        <p class="c3"><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 90.67px; height: 37.38px;"><img alt="" src="./images/image3.png" style="width: 90.67px; height: 37.38px; margin-left: -0.00px; margin-top: -0.00px; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px);" title=""></span></p>
                    </td>
                    <td class="c21" colspan="1" rowspan="1">
                        <p class="c6"><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 92.00px; height: 37.00px;"><img alt="" src="./images/image4.png" style="width: 92.00px; height: 37.00px; margin-left: 0.00px; margin-top: 0.00px; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px);" title=""></span></p>
                    </td>
                </tr>
            </tbody>
        </table>
        <p class="c18 c4"><span class="c0"></span></p>
        <p class="c18 c4"><span class="c0"></span></p>
    </div>
    <p class="c2"><span class="c0"></span></p>
    <p class="c15"><span class="c0"> {{doc.tipo}} </span></p>
    <p class="c19 c24"><span class="c0">EAJ, 09 de novembro de 2018</span></p>
    <p class="c2"><span class="c0"></span></p>
    <p class="c12"><span class="c9">De</span><span class="c0">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;: Ger&ecirc;ncia de Tecnologia da Informa&ccedil;&atilde;o</span></p>
    <p class="c12"><span class="c9">Para</span><span class="c0">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;: Coordena&ccedil;&atilde;o Rede e-tec Brasil</span></p>
    <p class="c12 c4"><span class="c0"></span></p>
    <p class="c12"><span class="c9">Assunto </span><span class="c0">: Verifica&ccedil;&atilde;o de status de equipamentos de inform&aacute;tica</span></p>
    <p class="c12 c4"><span class="c0"></span></p>
    <p class="c15 c22"><span class="c0">Segue abaixo a listagem de status dos equipamentos verificados pela Ger&ecirc;ncia de Tecnologia da Informa&ccedil;&atilde;o para a Coordena&ccedil;&atilde;o do E-tec.</span></p>
    <p class="c4 c7" id="h.gjdgxs"><span class="c0"></span></p>
    <p class="c20 c4"><span class="c0"></span></p>
    <p class="c20"><span class="c0">Switchs da Superintend&ecirc;ncia de Inform&aacute;tica - UFRN</span></p>
    <a id="t.688df099191b3e130f295e43306c23fd477a3d4f"></a>
    <a id="t.0"></a>
    <table class="c25">
        <tbody>
            <tr class="c13">
                <td class="c10" colspan="1" rowspan="1">
                    <p class="c3"><span class="c0">Patrim&ocirc;nio / MAC</span></p>
                </td>
                <td class="c5" colspan="1" rowspan="1">
                    <p class="c3"><span class="c0">Descri&ccedil;&atilde;o</span></p>
                </td>
                <td class="c16" colspan="1" rowspan="1">
                    <p class="c3"><span class="c0">Estado</span></p>
                </td>
            </tr>
            <tr v-for="item in itens" class="c13">
                <td class="c10" colspan="1" rowspan="1">
                    <p class="c3"><span class="c0">{{ item.patrimonio }}</span></p>
                </td>
                <td class="c5" colspan="1" rowspan="1">
                    <p class="c3"><span class="c0">{{ item.descricao }}</span></p>
                </td>
                <td class="c16" colspan="1" rowspan="1">
                    <p class="c3"><span class="c0">{{ item.estado }}</span></p>
                </td>
            </tr>
        </tbody>
    </table>
    <p class="c2 c22"><span class="c0"></span></p>
    <p class="c7 c4"><span class="c0"></span></p>
    <p class="c20"><span class="c0">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Atenciosamente,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span></p>
    <p class="c6"><span class="c0">____________________________</span></p>
    <p class="c19"><span class="c0">Onildo Braga de Oliveira</span></p>
    <p class="c19"><span class="c0">Coordenador do Suporte T&eacute;cnico em Inform&aacute;tica</span></p>
    <p class="c6"><span class="c0">SIAPE: 2135527</span></p>
    <p class="c19 c4"><span class="c0"></span></p>
    <div>
        <p class="c3"><span class="c8">RN 160 &ndash; Km 03 &ndash; Distrito de Jundia&iacute; &ndash; Maca&iacute;ba/RN &ndash; CEP 59.280-000 &ndash; Cx Postal 07</span></p>
        <p class="c3"><span class="c8">&nbsp;Fone/Fax (84) 3342-4802</span></p>
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld
  },
  data: () => ({
    doc: {},
    itens : [
    {}
    ],
    item: {}
  })
};
</script>

<style>
          .lst-kix_list_4-1>li {
            counter-increment: lst-ctn-kix_list_4-1
        }
        
        .lst-kix_list_5-1>li {
            counter-increment: lst-ctn-kix_list_5-1
        }
        
        ul.lst-kix_list_1-0 {
            list-style-type: none
        }
        
        .lst-kix_list_6-1>li {
            counter-increment: lst-ctn-kix_list_6-1
        }
        
        .lst-kix_list_3-0>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_3-1>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_3-2>li:before {
            content: "\002013  "
        }
        
        ol.lst-kix_list_6-6.start {
            counter-reset: lst-ctn-kix_list_6-6 0
        }
        
        .lst-kix_list_4-0>li {
            counter-increment: lst-ctn-kix_list_4-0
        }
        
        .lst-kix_list_5-0>li {
            counter-increment: lst-ctn-kix_list_5-0
        }
        
        .lst-kix_list_6-0>li {
            counter-increment: lst-ctn-kix_list_6-0
        }
        
        ul.lst-kix_list_1-3 {
            list-style-type: none
        }
        
        .lst-kix_list_3-5>li:before {
            content: "\002013  "
        }
        
        ul.lst-kix_list_1-4 {
            list-style-type: none
        }
        
        ul.lst-kix_list_1-1 {
            list-style-type: none
        }
        
        .lst-kix_list_3-4>li:before {
            content: "\002013  "
        }
        
        ul.lst-kix_list_1-2 {
            list-style-type: none
        }
        
        ul.lst-kix_list_1-7 {
            list-style-type: none
        }
        
        .lst-kix_list_3-3>li:before {
            content: "\002013  "
        }
        
        ul.lst-kix_list_1-8 {
            list-style-type: none
        }
        
        ul.lst-kix_list_1-5 {
            list-style-type: none
        }
        
        ul.lst-kix_list_1-6 {
            list-style-type: none
        }
        
        .lst-kix_list_3-8>li:before {
            content: "\002013  "
        }
        
        ol.lst-kix_list_5-3.start {
            counter-reset: lst-ctn-kix_list_5-3 0
        }
        
        .lst-kix_list_3-6>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_4-3>li {
            counter-increment: lst-ctn-kix_list_4-3
        }
        
        .lst-kix_list_3-7>li:before {
            content: "\002013  "
        }
        
        ol.lst-kix_list_4-5.start {
            counter-reset: lst-ctn-kix_list_4-5 0
        }
        
        ol.lst-kix_list_5-0.start {
            counter-reset: lst-ctn-kix_list_5-0 0
        }
        
        .lst-kix_list_5-2>li {
            counter-increment: lst-ctn-kix_list_5-2
        }
        
        ol.lst-kix_list_4-2.start {
            counter-reset: lst-ctn-kix_list_4-2 0
        }
        
        .lst-kix_list_5-0>li:before {
            content: "" counter(lst-ctn-kix_list_5-0, decimal) ". "
        }
        
        ol.lst-kix_list_6-0 {
            list-style-type: none
        }
        
        ol.lst-kix_list_6-1 {
            list-style-type: none
        }
        
        .lst-kix_list_5-4>li {
            counter-increment: lst-ctn-kix_list_5-4
        }
        
        .lst-kix_list_4-4>li {
            counter-increment: lst-ctn-kix_list_4-4
        }
        
        .lst-kix_list_4-8>li:before {
            content: " "
        }
        
        .lst-kix_list_5-3>li:before {
            content: "" counter(lst-ctn-kix_list_5-3, decimal) ". "
        }
        
        ol.lst-kix_list_6-4.start {
            counter-reset: lst-ctn-kix_list_6-4 0
        }
        
        .lst-kix_list_4-7>li:before {
            content: " "
        }
        
        .lst-kix_list_5-2>li:before {
            content: "" counter(lst-ctn-kix_list_5-2, lower-roman) ". "
        }
        
        .lst-kix_list_5-1>li:before {
            content: "" counter(lst-ctn-kix_list_5-1, lower-latin) ". "
        }
        
        .lst-kix_list_5-7>li:before {
            content: "" counter(lst-ctn-kix_list_5-7, lower-latin) ". "
        }
        
        ol.lst-kix_list_5-6.start {
            counter-reset: lst-ctn-kix_list_5-6 0
        }
        
        .lst-kix_list_5-6>li:before {
            content: "" counter(lst-ctn-kix_list_5-6, decimal) ". "
        }
        
        .lst-kix_list_5-8>li:before {
            content: "" counter(lst-ctn-kix_list_5-8, lower-roman) ". "
        }
        
        ol.lst-kix_list_4-1.start {
            counter-reset: lst-ctn-kix_list_4-1 0
        }
        
        ol.lst-kix_list_4-8.start {
            counter-reset: lst-ctn-kix_list_4-8 0
        }
        
        ol.lst-kix_list_6-6 {
            list-style-type: none
        }
        
        ol.lst-kix_list_6-7 {
            list-style-type: none
        }
        
        .lst-kix_list_5-4>li:before {
            content: "" counter(lst-ctn-kix_list_5-4, lower-latin) ". "
        }
        
        ol.lst-kix_list_6-8 {
            list-style-type: none
        }
        
        .lst-kix_list_5-5>li:before {
            content: "" counter(lst-ctn-kix_list_5-5, lower-roman) ". "
        }
        
        ol.lst-kix_list_6-2 {
            list-style-type: none
        }
        
        ol.lst-kix_list_6-3 {
            list-style-type: none
        }
        
        ol.lst-kix_list_6-4 {
            list-style-type: none
        }
        
        ol.lst-kix_list_6-5 {
            list-style-type: none
        }
        
        .lst-kix_list_6-1>li:before {
            content: "" counter(lst-ctn-kix_list_6-1, lower-latin) ". "
        }
        
        .lst-kix_list_6-3>li:before {
            content: "" counter(lst-ctn-kix_list_6-3, decimal) ". "
        }
        
        .lst-kix_list_6-5>li {
            counter-increment: lst-ctn-kix_list_6-5
        }
        
        .lst-kix_list_6-8>li {
            counter-increment: lst-ctn-kix_list_6-8
        }
        
        .lst-kix_list_6-0>li:before {
            content: "" counter(lst-ctn-kix_list_6-0, decimal) ") "
        }
        
        .lst-kix_list_6-4>li:before {
            content: "" counter(lst-ctn-kix_list_6-4, lower-latin) ". "
        }
        
        ol.lst-kix_list_4-0.start {
            counter-reset: lst-ctn-kix_list_4-0 0
        }
        
        ol.lst-kix_list_6-3.start {
            counter-reset: lst-ctn-kix_list_6-3 0
        }
        
        .lst-kix_list_6-2>li:before {
            content: "" counter(lst-ctn-kix_list_6-2, lower-roman) ". "
        }
        
        ol.lst-kix_list_5-5.start {
            counter-reset: lst-ctn-kix_list_5-5 0
        }
        
        .lst-kix_list_6-8>li:before {
            content: "" counter(lst-ctn-kix_list_6-8, lower-roman) ". "
        }
        
        .lst-kix_list_6-5>li:before {
            content: "" counter(lst-ctn-kix_list_6-5, lower-roman) ". "
        }
        
        .lst-kix_list_6-7>li:before {
            content: "" counter(lst-ctn-kix_list_6-7, lower-latin) ". "
        }
        
        .lst-kix_list_7-0>li:before {
            content: "  "
        }
        
        ol.lst-kix_list_4-7.start {
            counter-reset: lst-ctn-kix_list_4-7 0
        }
        
        .lst-kix_list_6-2>li {
            counter-increment: lst-ctn-kix_list_6-2
        }
        
        .lst-kix_list_6-6>li:before {
            content: "" counter(lst-ctn-kix_list_6-6, decimal) ". "
        }
        
        ol.lst-kix_list_5-0 {
            list-style-type: none
        }
        
        .lst-kix_list_2-6>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_2-7>li:before {
            content: "\002013  "
        }
        
        ol.lst-kix_list_5-1 {
            list-style-type: none
        }
        
        ol.lst-kix_list_5-2 {
            list-style-type: none
        }
        
        .lst-kix_list_7-4>li:before {
            content: "\0025ab  "
        }
        
        .lst-kix_list_7-6>li:before {
            content: "o  "
        }
        
        .lst-kix_list_2-4>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_2-5>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_2-8>li:before {
            content: "\002013  "
        }
        
        ol.lst-kix_list_6-2.start {
            counter-reset: lst-ctn-kix_list_6-2 0
        }
        
        .lst-kix_list_7-1>li:before {
            content: "\0025cf  "
        }
        
        .lst-kix_list_7-5>li:before {
            content: "\0025cf  "
        }
        
        .lst-kix_list_7-2>li:before {
            content: "o  "
        }
        
        .lst-kix_list_6-6>li {
            counter-increment: lst-ctn-kix_list_6-6
        }
        
        ol.lst-kix_list_5-4.start {
            counter-reset: lst-ctn-kix_list_5-4 0
        }
        
        .lst-kix_list_7-3>li:before {
            content: "\0025aa  "
        }
        
        ul.lst-kix_list_7-5 {
            list-style-type: none
        }
        
        ul.lst-kix_list_7-6 {
            list-style-type: none
        }
        
        ul.lst-kix_list_7-3 {
            list-style-type: none
        }
        
        ul.lst-kix_list_3-7 {
            list-style-type: none
        }
        
        ul.lst-kix_list_7-4 {
            list-style-type: none
        }
        
        ul.lst-kix_list_3-8 {
            list-style-type: none
        }
        
        ol.lst-kix_list_4-6.start {
            counter-reset: lst-ctn-kix_list_4-6 0
        }
        
        ol.lst-kix_list_5-1.start {
            counter-reset: lst-ctn-kix_list_5-1 0
        }
        
        ul.lst-kix_list_7-7 {
            list-style-type: none
        }
        
        ul.lst-kix_list_7-8 {
            list-style-type: none
        }
        
        ol.lst-kix_list_5-7 {
            list-style-type: none
        }
        
        .lst-kix_list_6-7>li {
            counter-increment: lst-ctn-kix_list_6-7
        }
        
        ul.lst-kix_list_3-1 {
            list-style-type: none
        }
        
        ol.lst-kix_list_5-8 {
            list-style-type: none
        }
        
        ul.lst-kix_list_3-2 {
            list-style-type: none
        }
        
        .lst-kix_list_5-7>li {
            counter-increment: lst-ctn-kix_list_5-7
        }
        
        .lst-kix_list_7-8>li:before {
            content: "\0025ab  "
        }
        
        ul.lst-kix_list_3-0 {
            list-style-type: none
        }
        
        ol.lst-kix_list_4-3.start {
            counter-reset: lst-ctn-kix_list_4-3 0
        }
        
        ol.lst-kix_list_5-3 {
            list-style-type: none
        }
        
        ul.lst-kix_list_7-1 {
            list-style-type: none
        }
        
        ul.lst-kix_list_3-5 {
            list-style-type: none
        }
        
        .lst-kix_list_4-7>li {
            counter-increment: lst-ctn-kix_list_4-7
        }
        
        ol.lst-kix_list_5-4 {
            list-style-type: none
        }
        
        ul.lst-kix_list_7-2 {
            list-style-type: none
        }
        
        ul.lst-kix_list_3-6 {
            list-style-type: none
        }
        
        ol.lst-kix_list_5-5 {
            list-style-type: none
        }
        
        ul.lst-kix_list_3-3 {
            list-style-type: none
        }
        
        ol.lst-kix_list_5-6 {
            list-style-type: none
        }
        
        ul.lst-kix_list_7-0 {
            list-style-type: none
        }
        
        .lst-kix_list_7-7>li:before {
            content: "\0025aa  "
        }
        
        ul.lst-kix_list_3-4 {
            list-style-type: none
        }
        
        .lst-kix_list_5-8>li {
            counter-increment: lst-ctn-kix_list_5-8
        }
        
        .lst-kix_list_4-0>li:before {
            content: " "
        }
        
        .lst-kix_list_4-1>li:before {
            content: " "
        }
        
        ol.lst-kix_list_6-8.start {
            counter-reset: lst-ctn-kix_list_6-8 0
        }
        
        .lst-kix_list_4-6>li {
            counter-increment: lst-ctn-kix_list_4-6
        }
        
        .lst-kix_list_4-4>li:before {
            content: " "
        }
        
        .lst-kix_list_4-3>li:before {
            content: " "
        }
        
        .lst-kix_list_4-5>li:before {
            content: " "
        }
        
        ol.lst-kix_list_6-5.start {
            counter-reset: lst-ctn-kix_list_6-5 0
        }
        
        .lst-kix_list_4-2>li:before {
            content: " "
        }
        
        .lst-kix_list_4-6>li:before {
            content: " "
        }
        
        ol.lst-kix_list_5-7.start {
            counter-reset: lst-ctn-kix_list_5-7 0
        }
        
        .lst-kix_list_5-5>li {
            counter-increment: lst-ctn-kix_list_5-5
        }
        
        ol.lst-kix_list_4-0 {
            list-style-type: none
        }
        
        ol.lst-kix_list_4-1 {
            list-style-type: none
        }
        
        ol.lst-kix_list_4-4.start {
            counter-reset: lst-ctn-kix_list_4-4 0
        }
        
        ol.lst-kix_list_4-2 {
            list-style-type: none
        }
        
        ol.lst-kix_list_4-3 {
            list-style-type: none
        }
        
        .lst-kix_list_6-4>li {
            counter-increment: lst-ctn-kix_list_6-4
        }
        
        ol.lst-kix_list_6-7.start {
            counter-reset: lst-ctn-kix_list_6-7 0
        }
        
        .lst-kix_list_6-3>li {
            counter-increment: lst-ctn-kix_list_6-3
        }
        
        .lst-kix_list_5-3>li {
            counter-increment: lst-ctn-kix_list_5-3
        }
        
        ul.lst-kix_list_2-8 {
            list-style-type: none
        }
        
        ol.lst-kix_list_4-8 {
            list-style-type: none
        }
        
        ol.lst-kix_list_6-1.start {
            counter-reset: lst-ctn-kix_list_6-1 0
        }
        
        ul.lst-kix_list_2-2 {
            list-style-type: none
        }
        
        .lst-kix_list_1-0>li:before {
            content: "\002013  "
        }
        
        ul.lst-kix_list_2-3 {
            list-style-type: none
        }
        
        ul.lst-kix_list_2-0 {
            list-style-type: none
        }
        
        ul.lst-kix_list_2-1 {
            list-style-type: none
        }
        
        ol.lst-kix_list_4-4 {
            list-style-type: none
        }
        
        ul.lst-kix_list_2-6 {
            list-style-type: none
        }
        
        ol.lst-kix_list_4-5 {
            list-style-type: none
        }
        
        .lst-kix_list_1-1>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_1-2>li:before {
            content: "\002013  "
        }
        
        ul.lst-kix_list_2-7 {
            list-style-type: none
        }
        
        ol.lst-kix_list_4-6 {
            list-style-type: none
        }
        
        ul.lst-kix_list_2-4 {
            list-style-type: none
        }
        
        ol.lst-kix_list_4-7 {
            list-style-type: none
        }
        
        ul.lst-kix_list_2-5 {
            list-style-type: none
        }
        
        .lst-kix_list_1-3>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_1-4>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_4-8>li {
            counter-increment: lst-ctn-kix_list_4-8
        }
        
        .lst-kix_list_1-7>li:before {
            content: "\002013  "
        }
        
        ol.lst-kix_list_5-8.start {
            counter-reset: lst-ctn-kix_list_5-8 0
        }
        
        .lst-kix_list_1-5>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_1-6>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_5-6>li {
            counter-increment: lst-ctn-kix_list_5-6
        }
        
        .lst-kix_list_2-0>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_2-1>li:before {
            content: "\002013  "
        }
        
        ol.lst-kix_list_6-0.start {
            counter-reset: lst-ctn-kix_list_6-0 0
        }
        
        .lst-kix_list_4-5>li {
            counter-increment: lst-ctn-kix_list_4-5
        }
        
        .lst-kix_list_1-8>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_2-2>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_2-3>li:before {
            content: "\002013  "
        }
        
        .lst-kix_list_4-2>li {
            counter-increment: lst-ctn-kix_list_4-2
        }
        
        ol.lst-kix_list_5-2.start {
            counter-reset: lst-ctn-kix_list_5-2 0
        }
        
        ol {
            margin: 0;
            padding: 0
        }
        
        table td,
        table th {
            padding: 0
        }
        
        .c16 {
            border-right-style: solid;
            padding: 0pt 5.4pt 0pt 5.4pt;
            border-bottom-color: #000000;
            border-top-width: 1pt;
            border-right-width: 1pt;
            border-left-color: #000000;
            vertical-align: middle;
            border-right-color: #000000;
            border-left-width: 1pt;
            border-top-style: solid;
            border-left-style: solid;
            border-bottom-width: 1pt;
            width: 176.6pt;
            border-top-color: #000000;
            border-bottom-style: solid
        }
        
        .c1 {
            border-right-style: solid;
            padding: 0pt 5.4pt 0pt 5.4pt;
            border-bottom-color: #000000;
            border-top-width: 1pt;
            border-right-width: 1pt;
            border-left-color: #000000;
            vertical-align: top;
            border-right-color: #000000;
            border-left-width: 1pt;
            border-top-style: solid;
            border-left-style: solid;
            border-bottom-width: 1pt;
            width: 176.6pt;
            border-top-color: #000000;
            border-bottom-style: solid
        }
        
        .c21 {
            border-right-style: solid;
            padding: 0pt 5.4pt 0pt 5.4pt;
            border-bottom-color: #000000;
            border-top-width: 0pt;
            border-right-width: 0pt;
            border-left-color: #000000;
            vertical-align: bottom;
            border-right-color: #000000;
            border-left-width: 0pt;
            border-top-style: solid;
            border-left-style: solid;
            border-bottom-width: 0pt;
            width: 144pt;
            border-top-color: #000000;
            border-bottom-style: solid
        }
        
        .c5 {
            border-right-style: solid;
            padding: 0pt 5.4pt 0pt 5.4pt;
            border-bottom-color: #000000;
            border-top-width: 1pt;
            border-right-width: 1pt;
            border-left-color: #000000;
            vertical-align: middle;
            border-right-color: #000000;
            border-left-width: 1pt;
            border-top-style: solid;
            border-left-style: solid;
            border-bottom-width: 1pt;
            width: 130.4pt;
            border-top-color: #000000;
            border-bottom-style: solid
        }
        
        .c17 {
            border-right-style: solid;
            padding: 0pt 5.4pt 0pt 5.4pt;
            border-bottom-color: #000000;
            border-top-width: 0pt;
            border-right-width: 0pt;
            border-left-color: #000000;
            vertical-align: bottom;
            border-right-color: #000000;
            border-left-width: 0pt;
            border-top-style: solid;
            border-left-style: solid;
            border-bottom-width: 0pt;
            width: 143.9pt;
            border-top-color: #000000;
            border-bottom-style: solid
        }
        
        .c10 {
            border-right-style: solid;
            padding: 0pt 5.4pt 0pt 5.4pt;
            border-bottom-color: #000000;
            border-top-width: 1pt;
            border-right-width: 1pt;
            border-left-color: #000000;
            vertical-align: middle;
            border-right-color: #000000;
            border-left-width: 1pt;
            border-top-style: solid;
            border-left-style: solid;
            border-bottom-width: 1pt;
            width: 117.4pt;
            border-top-color: #000000;
            border-bottom-style: solid
        }
        
        .c2 {
            padding-top: 0pt;
            padding-bottom: 0pt;
            line-height: 1.5;
            orphans: 2;
            widows: 2;
            text-align: justify;
            height: 12pt
        }
        
        .c14 {
            color: #000000;
            font-weight: 400;
            text-decoration: none;
            vertical-align: baseline;
            font-size: 10pt;
            font-family: "Verdana";
            font-style: normal
        }
        
        .c26 {
            color: #000000;
            font-weight: 400;
            text-decoration: none;
            vertical-align: baseline;
            font-size: 8pt;
            font-family: "Times New Roman";
            font-style: normal
        }
        
        .c8 {
            color: #000000;
            font-weight: 400;
            text-decoration: none;
            vertical-align: baseline;
            font-size: 10pt;
            font-family: "Times New Roman";
            font-style: normal
        }
        
        .c11 {
            color: #000000;
            font-weight: 400;
            text-decoration: none;
            vertical-align: baseline;
            font-size: 3pt;
            font-family: "Arial";
            font-style: normal
        }
        
        .c7 {
            padding-top: 0pt;
            text-indent: 35.4pt;
            padding-bottom: 0pt;
            line-height: 1.0;
            orphans: 2;
            widows: 2;
            text-align: justify
        }
        
        .c0 {
            color: #000000;
            font-weight: 400;
            text-decoration: none;
            vertical-align: baseline;
            font-size: 12pt;
            font-family: "Times New Roman";
            font-style: normal
        }
        
        .c20 {
            padding-top: 0pt;
            padding-bottom: 0pt;
            line-height: 1.0;
            orphans: 2;
            widows: 2;
            text-align: justify
        }
        
        .c18 {
            padding-top: 0pt;
            padding-bottom: 0pt;
            line-height: 1.0;
            orphans: 2;
            widows: 2;
            text-align: left
        }
        
        .c19 {
            padding-top: 0pt;
            padding-bottom: 0pt;
            line-height: 1.5;
            orphans: 2;
            widows: 2;
            text-align: right
        }
        
        .c6 {
            padding-top: 0pt;
            padding-bottom: 0pt;
            line-height: 1.0;
            orphans: 2;
            widows: 2;
            text-align: right
        }
        
        .c15 {
            padding-top: 0pt;
            padding-bottom: 0pt;
            line-height: 1.5;
            orphans: 2;
            widows: 2;
            text-align: justify
        }
        
        .c12 {
            padding-top: 0pt;
            padding-bottom: 0pt;
            line-height: 1.5;
            orphans: 2;
            widows: 2;
            text-align: left
        }
        
        .c3 {
            padding-top: 0pt;
            padding-bottom: 0pt;
            line-height: 1.0;
            orphans: 2;
            widows: 2;
            text-align: center
        }
        
        .c25 {
            margin-left: -5.4pt;
            border-spacing: 0;
            border-collapse: collapse;
            margin-right: auto
        }
        
        .c23 {
            background-color: #ffffff;
            max-width: 424.9pt;
            padding: 70.8pt 85pt 70.8pt 85pt
        }
        
        .c24 {
            margin-left: 247.8pt;
            text-indent: -247.8pt
        }
        
        .c4 {
            height: 12pt
        }
        
        .c13 {
            height: 0pt
        }
        
        .c9 {
            font-weight: 700
        }
        
        .c22 {
            text-indent: 35.4pt
        }
        
        .title {
            padding-top: 24pt;
            color: #000000;
            font-weight: 700;
            font-size: 36pt;
            padding-bottom: 6pt;
            font-family: "Times New Roman";
            line-height: 1.0;
            page-break-after: avoid;
            orphans: 2;
            widows: 2;
            text-align: left
        }
        
        .subtitle {
            padding-top: 18pt;
            color: #666666;
            font-size: 24pt;
            padding-bottom: 4pt;
            font-family: "Georgia";
            line-height: 1.0;
            page-break-after: avoid;
            font-style: italic;
            orphans: 2;
            widows: 2;
            text-align: left
        }
        
        li {
            color: #000000;
            font-size: 12pt;
            font-family: "Times New Roman"
        }
        
        p {
            margin: 0;
            color: #000000;
            font-size: 12pt;
            font-family: "Times New Roman"
        }
        
        h1 {
            padding-top: 24pt;
            color: #000000;
            font-weight: 700;
            font-size: 24pt;
            padding-bottom: 6pt;
            font-family: "Times New Roman";
            line-height: 1.0;
            page-break-after: avoid;
            orphans: 2;
            widows: 2;
            text-align: left
        }
        
        h2 {
            padding-top: 18pt;
            color: #000000;
            font-weight: 700;
            font-size: 18pt;
            padding-bottom: 4pt;
            font-family: "Times New Roman";
            line-height: 1.0;
            page-break-after: avoid;
            orphans: 2;
            widows: 2;
            text-align: left
        }
        
        h3 {
            padding-top: 14pt;
            color: #000000;
            font-weight: 700;
            font-size: 14pt;
            padding-bottom: 4pt;
            font-family: "Times New Roman";
            line-height: 1.0;
            page-break-after: avoid;
            orphans: 2;
            widows: 2;
            text-align: left
        }
        
        h4 {
            padding-top: 12pt;
            color: #000000;
            font-weight: 700;
            font-size: 12pt;
            padding-bottom: 2pt;
            font-family: "Times New Roman";
            line-height: 1.0;
            page-break-after: avoid;
            orphans: 2;
            widows: 2;
            text-align: left
        }
        
        h5 {
            padding-top: 11pt;
            color: #000000;
            font-weight: 700;
            font-size: 11pt;
            padding-bottom: 2pt;
            font-family: "Times New Roman";
            line-height: 1.0;
            page-break-after: avoid;
            orphans: 2;
            widows: 2;
            text-align: left
        }
        
        h6 {
            padding-top: 10pt;
            color: #000000;
            font-weight: 700;
            font-size: 10pt;
            padding-bottom: 2pt;
            font-family: "Times New Roman";
            line-height: 1.0;
            page-break-after: avoid;
            orphans: 2;
            widows: 2;
            text-align: left
        }
</style>

