# Bienvenue sur mon GitHub 👋

Un développeur passionné par le <span class="typewrite" data-period="2000" data-type='[ "web", "mobile", "backend" ]'><span class="wrap"></span></span>.

Actuellement étudiant en 2e année de **Génie Logiciel** à l'Institut Ivoirien de Technologie, je travaille sur plusieurs projets avec des technologies comme **HTML/CSS/JS**, **Flutter**, **Django**, et je fais aussi du **web scraping** avec **Selenium**.

<style>
.typewrite > .wrap { border-right: 0.08em solid #fff; }
</style>
<script>
var TxtType = function(el, toRotate, period) {
    this.toRotate = toRotate;
    this.el = el;
    this.loopNum = 0;
    this.period = parseInt(period, 10) || 2000;
    this.txt = '';
    this.tick();
    this.isDeleting = false;
};

TxtType.prototype.tick = function() {
    var i = this.loopNum % this.toRotate.length;
    var fullTxt = this.toRotate[i];

    if (this.isDeleting) {
    this.txt = fullTxt.substring(0, this.txt.length - 1);
    } else {
    this.txt = fullTxt.substring(0, this.txt.length + 1);
    }

    this.el.innerHTML = '<span class="wrap">'+this.txt+'</span>';

    var that = this;
    var delta = 200 - Math.random() * 100;

    if (this.isDeleting) { delta /= 2; }

    if (!this.isDeleting && this.txt === fullTxt) {
    delta = this.period;
    this.isDeleting = true;
    } else if (this.isDeleting && this.txt === '') {
    this.isDeleting = false;
    this.loopNum++;
    delta = 500;
    }

    setTimeout(function() {
    that.tick();
    }, delta);
};

window.onload = function() {
    var elements = document.getElementsByClassName('typewrite');
    for (var i=0; i<elements.length; i++) {
        var toRotate = elements[i].getAttribute('data-type');
        var period = elements[i].getAttribute('data-period');
        if (toRotate) {
          new TxtType(elements[i], JSON.parse(toRotate), period);
        }
    }
};
</script>

## Technologies & Compétences 🚀

- **Web Development**: HTML, CSS, JavaScript,Bootstrap
- **Mobile Development**: Dart/Flutter
- **Backend**: Python/Django
- **Web Scraping**: Selenium
- **Autres**: Git, GitHub, JSON,

## Contact 📫

Vous pouvez me contacter via:
- **Email**: kouadioazania@gmail.com
- **LinkedIn**: Azania kouadio

Merci de visiter mon GitHub et de jeter un œil à mes projets. N'hésitez pas à contribuer ou à me contacter pour discuter !
