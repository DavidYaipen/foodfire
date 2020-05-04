<template>
  <div>
    <article class="message">
      <section class="message-body">
        <div>
          <div class="media-content">
            <div class="webrow">
              <div class="columns is-mobile">
                <div class="column">
                  <p class="grey">Tiempo de Delivery</p>
                  <div>45 minutos</div>
                </div>
                <div class="column pl-10">
                  <p class="grey">Delivery Gratis</p>
                  <div class="w-132">above {{ 50 | currency }}</div>
                </div>
              </div>
              <div class="columns is-mobile">
                <div class="column">
                  <p class="grey">Horas de Delivery</p>
                  <div class="w-132">11:30AM - 10:30PM</div>
                </div>
                <div class="column pl-10">
                  <p class="grey">Minima Orden</p>
                  <div>{{ 2 | currency }}</div>
                </div>
              </div>
            </div>
            <div class="green">
              <center>
                <b>La entrega ya está abierta</b>
              </center>
            </div>
          </div>
        </div>
      </section>
    </article>
  </div>
</template>
<script>
export default {}
</script>
<style scoped>
.message {
  background-color: #f5f5f5;
  border-radius: 4px;
  font-size: 1rem;
}
.message-body {
  border-radius: 4px;
  border: solid #dbdbdb;
  border-width: 0 0 0 0px;
  color: #4a4a4a;
  padding: 1.25em 1.5em;
}
.media-content {
  flex-basis: auto;
  flex-grow: 1;
  flex-shrink: 1;
  text-align: left;
  padding-top: 23px;
}
@media (min-width: 900px) and (max-width: 2000px) {
  .w-132 {
    width: 132px;
  }
}
@media (min-width: 900px) and (max-width: 2000px) {
  .pl-10 {
    padding-left: 40px;
  }
}
@media (min-width: 900px) and (max-width: 2000px) {
  .columns.is-mobile {
    display: flex;
    flex-direction: row;
  }
}
@media (min-width: 900px) and (max-width: 2000px) {
  .webrow {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
  }
}
.columns.is-mobile {
  display: flex;
}
.column {
  display: block;
  flex-basis: 0;
  flex-grow: 1;
  flex-shrink: 1;
}
.grey {
  color: grey;
}
.green {
  color: green;
  margin-top: 1.5rem;
}
@media (min-width: 900px) and (max-width: 2000px) {
  .green {
    margin-top: -1.5rem;
  }
}
p {
  margin-bottom: 5px;
}
</style>
