Bootstrap 5-Column Layout
==================

Twitter Bootstrap does not provide grid system that allows us to create five columns layout, here is a bit of code that can make that happen.

Source:
https://github.com/twbs/bootstrap

At first you need to create default column definition in the way that Bootstrap do it. I called my classes col-..-15.

Add these CSS styles to your project:

<style>
.col-xs-15,
.col-sm-15,
.col-md-15,
.col-lg-15 {
    position: relative;
    min-height: 1px;
    padding-right: 10px;
    padding-left: 10px;
}


.col-xs-15 {
    width: 20%;
    float: left;
}
@media (min-width: 768px) {
.col-sm-15 {
        width: 20%;
        float: left;
    }
}
@media (min-width: 992px) {
    .col-md-15 {
        width: 20%;
        float: left;
    }
}
@media (min-width: 1200px) {
    .col-lg-15 {
        width: 20%;
        float: left;
    }
}
</style>

Reference Your New Classes:

<div class="row"><div class="col-md-15 col-sm-3"></div></div>
