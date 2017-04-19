transform是一个为IE6-8提供css3 transform属性功能的js库，它的使用非常简单
jquery方式/jquery way:

<!--[if lte IE 8]>
    <script src="build/jquery.transform.js"></script>
<![endif]-->
<script>
jQuery(function($) {
    $(".test").css("transform", "rotate(45deg)");
});
</script>

或htc方式/Or htc way:

<style>
.test {
    -webkit-transform: rotate(45deg);
    -ms-transform: rotate(45deg);
    transform: rotate(45deg);
    behavior: url(build/transform.htc);
}
</style>

