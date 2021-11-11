https://diegomariano.com/compilando-o-bootstrap-com-sass-e-npm/

your-project/
├── scss
│   └── custom.scss
└── node_modules/
    └── bootstrap
        ├── js
        └── scss
		
		
criar pasta
npm init
npm install bootstrap
npm install jquery
npm install -g sass

cria o arquivo da index

<!doctype html>
<html lang="pt-br">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!-- Bootstrap CSS -->
    <link href="node_modules/bootstrap/dist/css/bootstrap.css" rel="stylesheet" />

     <title class="">Hello, world!</title>
  </head>
  <body>
    <h1>Hello, world!</h1>

  </body>
</html>
Cria a pasta CSS 

Para compilar
> sass --watch .\node_modules\bootstrap\scss:.\css\bootstrap\

ESTILO

sass --watch .\scss\estilo.scss:.\css\estilo.css

Navigate to the root /bootstrap directory and run npm install to install our local dependencies listed in package.json.

https://getbootstrap.com/docs/5.1/customize/sass/


// Custom.scss
// Option A: Include all of Bootstrap

// Include any default variable overrides here (though functions won't be available)

@import "../node_modules/bootstrap/scss/bootstrap";

// Then add additional custom code here

---------------

Breakpoint	Class infix	Dimensions
X-Small	None	<576px
Small	sm	≥576px
Medium	md	≥768px
Large	lg	≥992px
Extra large	xl	≥1200px
Extra extra large	xxl	≥1400px

$grid-breakpoints: (
  xs: 0,
  sm: 576px,
  md: 768px,
  lg: 992px,
  xl: 1200px,
  xxl: 1400px
);

SASS
$container-max-widths: (
  sm: 540px,
  md: 720px,
  lg: 960px,
  xl: 1140px,
  xxl: 1320px
);

xs
<576px	sm
≥576px	md
≥768px	lg
≥992px	xl
≥1200px	xxl
≥1400px

Container max-width	None (auto)	540px	720px	960px	1140px	1320px
Class prefix	.col-	.col-sm-	.col-md-	.col-lg-	.col-xl-	.col-xxl-
# of columns	12
Gutter width	1.5rem (.75rem on left and right)