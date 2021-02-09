<template class="background">
<q-page>
    <div class="row justify-center mgt" align="center">
      <div class="col-4"></div>
      <div class="col-4">
       <form method="get">
         <div class="row">
           <div class="col">
            <input type="text" name="url" placeholder=" URL" class="input">
          </div>
         </div>
         <div class="row">
           <div class="col">
            <input type="text" name="titulo" placeholder=" Título" class="input mgt-20">
          </div>
          </div>
          <div class="row">
           <div class="col">
            <input type="text" name="codsec" placeholder=" Código de Segurança" class="input mgt-20">
          </div>
          </div>
          <div class="row">
           <div class="col">
            <input type="text" name="referencias" placeholder=" Referências" class="input-2 mgt-20" style="margin-right: 10px">
          </div>
          <div class="col">
            <input type="text" name="ordem" placeholder=" Ordem" class="input-2 mgt-20" style="margin-left: 10px;">
          </div>
          </div>
          <div class="row">
            <div class="col">
              <select id="materias" name="materias" class="input mgt-20">
                  <option value="humanas">Humanas</option>
                  <option value="natureza">Natureza</option>
                  <option value="matematica">Matemática</option>
                  <option value="linguagens">Linguagens</option>
                  <option value="concursos">Concursos</option>
                  <option value="faculdade">Faculdade</option>
                  <option value="economia">Educação Financeira</option>
                  <option value="sustentabilidade">Sustentabilidade</option>
                  <option value="digital">Produção Digital</option>
                  <option value="saude">Saúde</option>
                  <option value="politica">Política</option>
                  <option value="linguistica">Linguistica</option>
                  <option value="avulsos">Avulsos</option>
                  <option value="pessoal">Des. Pessoal</option>
                  <option value="profissional">Des. Profissional</option>
              </select>
            </div>
          </div>
       </form>
      <div>
        <q-btn label="Enviar" type="submit" color="warning" class="input mgt-20"/>
      </div>
      </div>
      <div class="col-4"></div>
    </div>
</q-page>
</template>
<style lang="sass">
  .background
    background-color: white
  .mgt
    margin-top: 100px
  .input
    width: 100%
    height: 40px
  .input-2
    width: 95%
    height: 40px
  .mgt-20
    margin-top: 20px
</style>
