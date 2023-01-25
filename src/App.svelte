<script>
  import Barra from "./lib/Barra.svelte"
  import Content from "./lib/Content.svelte"
</script>

<main id="page-top">
  <div id="wrapper">
    <Barra/>
    <div class="d-flex flex-column" id="content-wrapper">
        <Content/>
        <footer class="bg-white sticky-footer">
            <div class="container my-auto">
                <div class="text-center my-auto copyright mt-1"><span>Copyright © Sebastian Felipe Herrera Varela 2023</span></div>
            </div>
            <div class="container my-auto">
                <div class="text-center my-auto copyright mt-1"><span>Desarrollado en el area de Transmision y Distribucion</span></div>
            </div>
        </footer>
    </div><a class="border rounded d-inline scroll-to-top" href="#page-top"><i class="fas fa-angle-up"></i></a>
</div>
</main>

<style>
</style>
