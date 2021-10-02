## Hi! Sou José Augusto Alcarás
 <div>
<div align="center">
  <a href="https://github.com/JAlcaras">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=JAlcaras&show_icons=true&theme=dark&include_all_commits=true&count_private=true"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=JAlcaras&layout=compact&langs_count=7&theme=dark"/>
</div>

<h4 align="center"> 
	🚧  Perfil 🚀 Em construção...  🚧
</h4>


<iframe width="100%" height="100%" 
        src="https://www.youtube.com/embed/mdWHYvQoY8g" 
        frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
</iframe>
 
<!-- Css -->
<style>
  @import 'https://fonts.googleapis.com/css?family=Ubuntu';
  body {
    background: #bdc3c7;
    font-family: 'Ubuntu', sans-serif;
    font-size: 17px;
  }

  .window {
    width: 600px;
    margin: 75px auto;
    background: #2c3e50;
    height: 350px;
    border-radius: 5px;
    display: relative;
    box-shadow: 10px 10px 10px #888888;
  }

  .afterclose {
    color: #34495e;
    display: none;
    text-align: center;
  }

  .open {
    color: #fff;
    padding: 15px;
    background: #2ecc71;
    border-radius: 4px;
    border: none;
  }

  .bash {
    width: 600px;
    background: #34495e;
    height: 310px;
    border-radius: 5px;
    top: 40px;
    display: absolute;
    color: #fff;
  }

  /* effected by controllers */

  .windowmax {
    width: 100%;
    margin: auto;
    background: #2c3e50;
    height: 1000px;
    border-radius: 5px;
    display: relative;
  }

  .windowmin {
    width: 300px;
    height: 45px;
    background: #2c3e50;
    border-radius: 5px;
    bottom: 0;
    position: fixed;
  }

  .bashmax {
    display: absolute;
    width: 100%;
    background: #34495e;
    height: 960px;
    border-radius: 5px;
    bottom: 0;
    color: #fff;
  }

  /* !--end--! */

  .buttons {
    width: 15px;
    height: 15px;
    border-radius: 50%;
    float: right;
    margin: 13px 4px;
    border: none;
  }

  .close {
    background: #e74c3c;
  }

  .maximize {
    background: #f1c40f;
  }

  .minimize {
    background: #2ecc71;
  }

  .result {
    display: none;
  }

  .controls {
    height: 40px;
    top: 0;
  }

  .title {
    color: #fff;
    font-weight: bold;
    padding: 10px;
  }
</style>
<!-- HTML -->
<h1 class="afterclose">
  You Closed Terminal ! --> <button class="open">reopen ?</button>
</h1>
<div class="window">
  <div class="controls">
    <button class="buttons close" id="close"></button>
    <button class="buttons maximize" href="#"></button>
    <button class="buttons minimize" href="#"></button>
    <div class="title">Gnome Terminal</div>
  </div>
  <div class="bash">
    <!-- Terminal sem comando -->
    <span class="span">[adnan@linux-pc ~]:$</span>
    <br />
    <!-- Terminal com comando -->
    <span class="span">[adnan@linux-pc ~]:$</span>
    <span class="type-it">dnf update</span>
    <br />
    <div class="result">
      <span id="span2"> ola mundo root</span>
      <br />
    </div>
  </div>
</div>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<script src="https://cdn.jsdelivr.net/jquery.typeit/4.2.3/typeit.min.js"></script>
<!-- Scripts -->
<script>
  $('.type-it').typeIt({})
  //detected terminal words
  var span = $('.span')
  span.html(
    span
      .html()
      .replace(
        /adnan/,
        '<span style="color: #3498db ; font-weight: bold; ">$&</span>'
      )
  )

  var span = $('.span')
  span.html(
    span
      .html()
      .replace(
        /~/,
        '<span style="color: #2ecc71 ; font-weight: bold; ">$&</span>'
      )
  )

  var span = $('#span2')
  span.html(
    span
      .html()
      .replace(
        /root/,
        '<span style="color: #e74c3c ; font-weight: bold; ">$&</span>'
      )
  )

  var span = $('#span2')
  span.html(
    span
      .html()
      .replace(
        /Error/,
        '<span style="color: #e74c3c ; font-weight: bold; ">$&</span>'
      )
  )

  //result proccess
  setInterval(Timer, 3500)
  function Timer() {
    $('.result').show()
  }

  //controllers :D
  $('button.close').click(function () {
    $('.window').hide()
    $('.afterclose').fadeIn('fast')
  })

  $('button.open').click(function () {
    $('.window').show()
    $('.afterclose').hide()
  })

  $('button.maximize').click(function () {
    $('.window').addClass('windowmax')
    $('.bash').addClass('bashmax')
    $('.windowmax').removeClass('window')
    $('.bashmax').removeClass('bash')
  })

  $('button.minimize').click(function () {
    $('.bash').remove()
    $('.window').addClass('windowmin')
    $('.windowmin').removeClass('window')
  })
</script>

	
<div>
    <iframe src="https://github.com/JAlcaras/JAlcaras/blob/main/index_temrminal_v2.html" scrolling="no" frameborder="no"></iframe>
</div>	


	
	
