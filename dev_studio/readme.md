# Разработка приложений в DevStudio
Для начала хочу сказать что приложения в данной студии пишутся на языке HTML и требуется придерживаться некоторых правил а также учитывать то что контент должен быть цензурным. 

Для написания приложения должен быть стартовый шаблон:
```html
<div class='header'>
  <div class='button-back' onclick='closeApp()'>􀆉 Назад</div>
  <div class='app-name'>My First App</div>
</div>
<div class='container'>
  <h3>My Firts App</h3>
  <p>Это мое первое приложение написанное в DevStudio</p>
</div>
```
<image
  src="static/screen1.png"
  alt="Скриншот из DevStudio"
  caption="Скриншот из DevStudio">
Полностью приложение пишется на языке HTML, в него можно встраивать JS код например:
```html
<div class='header'>
  <div class='button-back' onclick='closeApp()'>􀆉 Назад</div>
  <div class='app-name'>My First App</div>
</div>
<div class='container'>
  <h3>My Firts App</h3>
  <p>Это мое первое приложение написанное в DevStudio</p>
</div>

<script>
  window.addEventListener("DOMContentLoaded", ()=>{
    document.querySelector("p").innerHTML = "Изменено с помощью JavaScript"
    document.querySelector("p").style.background = "rgb(0, 122, 255)";
    document.querySelector("p").style.color = "white";
    document.querySelector("p").style.padding = "20px";
    document.querySelector("p").style.borderRadius = "10px";
    document.querySelector("p").style.cursor = "pointer"
    document.querySelector("p").style.textAlign = "center";
  	document.querySelector("p").onclick = () => {
      alert("hello, world!")
    }
  })
</script>
```
