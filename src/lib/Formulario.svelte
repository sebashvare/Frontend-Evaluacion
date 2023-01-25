<script>
    let orden = "";
    const prueba = (event) =>{
        orden = event.target.value;
        console.log(orden)
    }
    $: if (orden.length >= 10) {
        console.log(orden);
    }
    </script>

<div class="container-fluid">
        <h3 class="text-dark mb-4 text-gray-600 text-uppercase">Planeacion</h3>
        <div class="card shadow">
            <div class="card-header py-3">
                <p class="text-primary m-0 fw-bold text-gray-500 text-uppercase">Informacion Planeacion</p>
            </div>
            <div class="card-body">
                <div class="row">
                    <div class="col prueba">
                        <div class="input-group mt-3">
                            <span class="input-group-text"><i class="fa fa-search"></i></span>
                            <input class="form-control form-control-sm" bind:value={orden} on:change={prueba} type="number" placeholder="Ingrese la ORDEN ...">
                        </div>
                        <div class="input-group mt-2"><span class="input-group-text"><i class="fa fa-info"></i></span><input class="form-control form-control-sm" type="number" placeholder="ID de cuenta"></div>
                        <div class="input-group mt-2"><span class="input-group-text"><i class="fa fa-info"></i></span><input class="form-control form-control-sm" type="number" placeholder="Nombre de cuenta"></div>
                        <div class="input-group mt-2"><span class="input-group-text"><i class="fa fa-info"></i></span><input class="form-control form-control-sm" type="text" placeholder="Fuente"></div>
                        <div class="input-group mt-2"><span class="input-group-text"><i class="fa fa-info"></i></span><input class="form-control form-control-sm" type="text" placeholder="Contrata"></div>
                        <div class="input-group mt-2"><span class="input-group-text"><i class="fa fa-info"></i></span><select class="form-select form-select-sm">
                                <optgroup label="Tipo de actividad">
                                    <option value="12">This is item 1</option>
                                    <option value="13">This is item 2</option>
                                    <option value="14">This is item 3</option>
                                </optgroup>
                            </select></div><small class="form-text mt-1">* Seleccione el tipo de Actividad.</small>
                        <div class="input-group mt-1"><button class="btn btn-primary" id="guardar-info" type="button">Guardar Informacion</button></div>
                    </div>
                </div>
            </div>
        </div>
    </div>