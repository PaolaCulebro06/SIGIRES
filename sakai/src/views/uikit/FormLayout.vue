<template>
  <div class="grid">
    <div class="col-12 md:12">
      <div class="card p-fluid">
        <div class="card-body">
          <h4 class="card-title">Inventario Almacén 1</h4>
          <div class="table-responsive">
            <table class="table table-bordered table-striped">
              <thead>
                <tr>
                  <th>No. de Inventario</th>
                  <th>Nombre</th>
                  <th>Marca</th>
                  <th>Formula</th>
                  <th>PM</th>
                  <th>Capacidad del recipiente</th>
                  <th>Recipientes actuales</th>
                  <th>Lote</th>
                  <th>Contenido aproximado</th>
                </tr>
              </thead>
              <tbody>
                <!-- <tr v-for="platillo in platillos" :key="platillo.id">
                  <td>{{ platillo.id }}</td>
                  <td>{{ platillo.nombre }}</td>
                  <td>{{ formatCurrency(platillo.precio) }}</td>
                  <td> -->
                    <!-- <button class="btn btn-success btn-sm" @click="editarPlatillo(platillo)">Editar</button>
                    <button class="btn btn-danger btn-sm" @click="eliminarPlatillo(platillo)">Eliminar</button> -->
                  <!-- </td>
                </tr> -->
              </tbody>
            </table>
          </div>
        </div>
        <div class="card-footer">
          <button class="btn btn-primary" @click="agregarAlmacen1">Agregar </button>
          <button class="btn btn-success btn-sm" @click="editarAlmacen1(platillo)">Editar</button>
          <button class="btn btn-danger btn-sm" @click="eliminarAlmacen1(platillo)">Eliminar</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>

// const platillos = ref([
//   { id: 1, nombre: 'Platillo 1', descripcion: 'Descripción del Platillo 1', precio: 10.99 },
//   { id: 2, nombre: 'Platillo 2', descripcion: 'Descripción del Platillo 2', precio: 15.99 },
//   { id: 3, nombre: 'Platillo 3', descripcion: 'Descripción del Platillo 3', precio: 8.99 },
// ]);

const formatCurrency = (value) => {
  return value.toLocaleString('en-US', { style: 'currency', currency: 'USD' });
};

const agregarAlmacen1 = () => {
  // Lógica para agregar un nuevo ....
};

const editarAlmacen1= (nombre) => {
  // Editar ingreso ...
};

const eliminarAlmacen1 = (nombre) => {
  // Lógica para eliminar un ...
};
</script>

<style scoped>
.table {
  width: 100%;
  margin-bottom: 1rem;
  color: #212529;
  border-collapse: collapse;
}

.table th,
.table td {
  padding: 0.75rem;
  vertical-align: top;
  border-top: 1px solid #dee2e6;
}

.table thead th {
  vertical-align: bottom;
  border-bottom: 2px solid #dee2e6;
}

.table tbody + tbody {
  border-top: 2px solid #dee2e6;
}

.table-sm th,
.table-sm td {
  padding: 0.3rem;
}

.btn {
  display: inline-block;
  font-weight: 400;
  color: #212529;
  text-align: center;
  vertical-align: middle;
  cursor: pointer;
  background-color: transparent;
  border: 1px solid transparent;
  padding: 0.375rem 0.75rem;
  font-size: 1rem;
  line-height: 1.5;
  border-radius: 0.25rem;
  transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out,
    border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
}

.btn-primary {
  color: #fff;
  background-color: #007bff;
  border-color: #007bff;
}

.btn-success {
  color: #fff;
  background-color: #28a745;
  border-color: #28a745;
}

.btn-danger {
  color: #fff;
  background-color: #dc3545;
  border-color: #dc3545;
}

.btn-sm {
  padding: 0.25rem 0.5rem;
  font-size: 0.875rem;
  line-height: 1.5;
  border-radius: 0.2rem;
}
</style>


