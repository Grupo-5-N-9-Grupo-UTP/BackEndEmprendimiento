<template>
    <div class="container">
        <div class="form">
            <span class="circle one"></span>
            <span class="circle two"></span>
            <div class="pasos">
                <div class="paso">
                    <h2>PASO 1</h2>
                    <h4>Idea de negocio</h4>
                    <div class="iconos">
                        <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-bulb" width="84"
                            height="84" viewBox="0 0 24 24" stroke-width="1.5" stroke="#6F4C5B" fill="none"
                            stroke-linecap="round" stroke-linejoin="round">
                            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                            <path d="M3 12h1m8 -9v1m8 8h1m-15.4 -6.4l.7 .7m12.1 -.7l-.7 .7" />
                            <path d="M9 16a5 5 0 1 1 6 0a3.5 3.5 0 0 0 -1 3a2 2 0 0 1 -4 0a3.5 3.5 0 0 0 -1 -3" />
                            <line x1="9.7" y1="17" x2="14.3" y2="17" />
                        </svg>
                    </div>
                    <p>Para esto el emprendedor puede utilizar el cuadro DOFA-CANVAS Y PESTEL, como herramnientas para
                        identificar aspectos claves de su negocio</p>
                    <br>
                    <input type="submit" value="ver más" class="btn-invertido" />
                    <br>
                </div>

                <div class="paso">
                    <h2>PASO 2</h2>
                    <h4>Plan empresarial</h4>
                    <div class="iconos">
                        <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-businessplan" width="84px"
                            height="84px" viewBox="0 0 24 24" stroke-width="1.5" stroke="#6F4C5B" fill="none"
                            stroke-linecap="round" stroke-linejoin="round">
                            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                            <ellipse cx="16" cy="6" rx="5" ry="3" />
                            <path d="M11 6v4c0 1.657 2.239 3 5 3s5 -1.343 5 -3v-4" />
                            <path d="M11 10v4c0 1.657 2.239 3 5 3s5 -1.343 5 -3v-4" />
                            <path d="M11 14v4c0 1.657 2.239 3 5 3s5 -1.343 5 -3v-4" />
                            <path d="M7 9h-2.5a1.5 1.5 0 0 0 0 3h1a1.5 1.5 0 0 1 0 3h-2.5" />
                            <path d="M5 15v1m0 -8v1" />
                        </svg>
                    </div>
                    <p>Aquí es importante que describa el producto o servicio que como empresa va a ofrecer y a su vez
                        planifiquen sus objetivos </p>
                    <br>
                    <input type="submit" value="ver más" class="btn-invertido" />
                    <br>
                </div>

                <div class="paso">
                    <h2>PASO 3</h2>
                    <h4>Clasificación de la empresa</h4>
                    <div class="iconos">
                        <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-building-skyscraper"
                            width="84" height="84" viewBox="0 0 24 24" stroke-width="1.5" stroke="#6F4C5B" fill="none"
                            stroke-linecap="round" stroke-linejoin="round">
                            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                            <line x1="3" y1="21" x2="21" y2="21" />
                            <path d="M5 21v-14l8 -4v18" />
                            <path d="M19 21v-10l-6 -4" />
                            <line x1="9" y1="9" x2="9" y2="9.01" />
                            <line x1="9" y1="12" x2="9" y2="12.01" />
                            <line x1="9" y1="15" x2="9" y2="15.01" />
                            <line x1="9" y1="18" x2="9" y2="18.01" />
                        </svg>
                    </div>
                    <p>Identificar si la empresa es pública privada o mixta y si es natural, juridica o un lugar de comercio</p>
                    <br>
                    <input type="submit" value="ver más" class="btn-invertido" />
                    <br>
                </div>

                <div class="paso">
                    <h2>PASO 4</h2>
                    <h4>Tipo de sociedad</h4>
                    <div class="iconos">
                        <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-users" width="84"
                            height="84" viewBox="0 0 24 24" stroke-width="1.5" stroke="#6F4C5B" fill="none"
                            stroke-linecap="round" stroke-linejoin="round">
                            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                            <circle cx="9" cy="7" r="4" />
                            <path d="M3 21v-2a4 4 0 0 1 4 -4h4a4 4 0 0 1 4 4v2" />
                            <path d="M16 3.13a4 4 0 0 1 0 7.75" />
                            <path d="M21 21v-2a4 4 0 0 0 -3 -3.85" />
                        </svg>
                    </div>
                    <p>Se puede clasificar en Limitada(LTDA)- Anonima(SA)-Por Acciones Simplificada(SAS)</p>
                    <br>
                    <input type="submit" value="ver más" class="btn-invertido" />
                    <br>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import '../assets/scripts/app.js'
export default {
  name: 'index-paso-a-paso',
  props: {
    msg: String
  }
}
</script>

<style>
   @import '../assets/styles/style.css';
</style>
