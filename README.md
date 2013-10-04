scrollzip
=========

jQuery plugin to trigger action if element is visible or hidden while scrolling.

    $(document).ready(function(){
      $(document).scrollzipInit();
      $(window).on("load scroll resize", function(){
          $('.section').scrollzip({
              showFunction    : function() { $(this).css("visibility", "visible").addClass('animated bounceInLeft'); },
              hideFunction    : function() { $(this).css("visibility", "hidden").removeClass('animated'); },
              //showShift       : 100,//optional
              //hideShift       : -100,//optional
              //wholeVisible  : true,//optional
          });
      )};
    )};
