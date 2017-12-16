#product images

{% assign featured_image = product.selected_or_first_available_variant.featured_image | default: product.featured_image %}
<div class="product_gallery product-{{ product.id }}-gallery {% if product-images == blank %}product_slider{% endif %} {% if settings.product_thumbs == false %}animated fadeInUp{% endif %}">
<div class="slider slider-for">
   {% for image in product.images %}
  <div>
<img class="img1" rel="gallery1" src="{{ image | product_img_url: '1024x1024' }}" data-zoom-image="{{ image | product_img_url: '1024x1024' }}" /> 
  </div>
  {%endfor%}
</div>
<div class="slider slider-nav">
   {% for image in product.images %}
  <div>
   <img  src="{{ image | product_img_url: '100x1000' }}">
  </div>
  {%endfor%}
</div>
</div>
 
 <script>
$(document).ready(function(){  
  $('.slider-for').slick({
  slidesToShow: 1,
  slidesToScroll: 1,
  arrows: false,
  fade: true,
  asNavFor: '.slider-nav'
});
$('.slider-nav').slick({
  slidesToShow: 3,
  slidesToScroll: 1,
  asNavFor: '.slider-for',
  dots: true,
  centerMode: true,
  focusOnSelect: true
});
  });
</script>
