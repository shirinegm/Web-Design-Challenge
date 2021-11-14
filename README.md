# Web-Design-Challenge
1. To use this website to display another dataset, first make sure the cities_weather_df.csv is under the Resources folder
1. Run the jupyter notebook generate_data.ipynb to format the data in the csv into html. Make sure the name of the csv file is updated in the jupyter notebook.
1. Copy the generated html code into the table element under <!--Data-->

# Bootstrap and Media Queries
1. This website uses the latest bootstrap version (bootstrap@5.1.3) installed using the bundle version placed right before the <\body> tag. If you need to update the bootstrap version, replace the bundle link with the new one from Bootstrap.
1. This website uses Bootswatch Superhero template (https://bootswatch.com/superhero/#top)
1. To use a different template, download the bootswatch.css file for the given template and replace the one in the root.
1. The Bootswatch templates have media queries for 5 sizes for navbar. I used navbar-expand-lg. Below is an extract from the bootswatch.css file specifically addressing how the navbar should behave below 992px width. The navbar also uses the navbar-nav class and that is included in all 5 media queries, telling the navbar how to behave below 1400px, 1200px, 992px, 768px and 576px. The instructions include, positioning, padding, visibility and height amongs others:

@media (min-width:992px){
	.navbar-expand-lg{-ms-flex-wrap:nowrap;flex-wrap:nowrap;-ms-flex-pack:start;justify-content:flex-start}
	.navbar-expand-lg .navbar-nav{-ms-flex-direction:row;flex-direction:row}
	.navbar-expand-lg .navbar-nav .dropdown-menu{position:absolute}
	.navbar-expand-lg .navbar-nav .nav-link{padding-right:.5rem;padding-left:.5rem}
	.navbar-expand-lg .navbar-nav-scroll{overflow:visible}
	.navbar-expand-lg .navbar-collapse{display:-ms-flexbox!important;display:flex!important;-ms-flex-preferred-size:auto;flex-basis:auto}
	.navbar-expand-lg .navbar-toggler{display:none}
	.navbar-expand-lg .offcanvas-header{display:none}
	.navbar-expand-lg .offcanvas{position:inherit;bottom:0;z-index:1000;-ms-flex-positive:1;flex-grow:1;visibility:visible!important;background-color:transparent;border-right:0;border-left:0;transition:none;-webkit-transform:none;transform:none}
	.navbar-expand-lg .offcanvas-bottom,.navbar-expand-lg .offcanvas-top{height:auto;border-top:0;border-bottom:0}
	.navbar-expand-lg .offcanvas-body{display:-ms-flexbox;display:flex;-ms-flex-positive:0;flex-grow:0;padding:0;overflow-y:visible}