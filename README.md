# Вывод ПОДКАТЕГОРИИ из текущей КАТЕГОРИИ

```php
<?php
if ( is_category() ) {
  if ( count(get_categories('child_of='.$cat)) )
    echo '<ul class="sub_categories">';
    $current_cat=get_query_var('cat');
    wp_list_categories('child_of='.$current_cat.'&title_li=&show_count=0&hide_empty=0'); 
    echo '</ul>';
}
?>
```
