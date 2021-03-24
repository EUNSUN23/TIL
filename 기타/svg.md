###bitmap
the most common bitmap image format for the web are JPEG,PNG and GIF.

- simply define what color each pixel of the image should be painted.
- well suit for highly detailed imageds, such as photograpsh.
- can be heavy for low-resolution devices or if they are connected to a low
  bandwidth work.

###svg

- vector image format for the web

- provide a set of instructions about how the image should be renderd. It's up to the rendering
  software to compute how each pixel should be colored.

- well suit for less detailed images that need to be scaled at different sizes like icons or
  data representations.

- useful when you want a single image to fit screens of so many different sizes and resolutions.

<IMPORTANT>
- it is a text format written with tags like HTML. 
- it can be styled with css like HTML. 
- it can be scripted with JavaScript like HTML.

\*\*HTML은 본래 문서 describing을 위해서 만들어진 것이고, SVG는 이미지 describing을 위해 만들어진것임.

svg로 하트 등 복잡한 이미지를 직접 만드려면 어려움.. Inskape, Illustrator, Sketch등이 svg작업용 소프트웨어 대표.
snap.svg, Bonsai, D3.js등의 svg용 자바스크립트 라이브러리도 있음.
