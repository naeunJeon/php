php 18.12.06

매개변수 전달 방식
1. 값 전달
2. 참조 전달
3. 디폴트 매개변수
4. 가변 길이 인수목록
```php
<?php
function sum(...$num){
    $sum = 0;
    foreach ($num as $item) {
        $sum += $item;
    }
    return $sum;
}
echo sum(1,2,3)
?>
```