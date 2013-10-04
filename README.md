scrollzip
=========

jQuery plugin to trigger action if element is visible or hidden while scrolling. 
This plugin is used to trigger some action if the given element is becoming visible or hidden while scrolling. 
The given [demo](http://demo.tinywall.net/scrollzip/) is using the [animate.css](http://daneden.me/animate/) for the visibility action.

    $(document).ready(function(){
      $(document).scrollzipInit();
      $(window).on("load scroll resize", function(){
          $('.section').scrollzip({
              showFunction    : function() { $(this).css("visibility", "visible").addClass('animated bounceInLeft'); },//optional
              hideFunction    : function() { $(this).css("visibility", "hidden").removeClass('animated'); },//optional
              //showShift       : 100,//optional
              //hideShift       : -100,//optional
              //wholeVisible  : true,//optional
          });
      )};
    )};
