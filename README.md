
> 根据ip，获取ip地址所在的地理位置信息
> 基于纯真ip数据库

## ip库最新更新时间
2018年5月10日

## 安装

```json
{
    "require": {
        "pouduo/iplocation": "^1.0",
    }
}
```

or

Require this package with composer:
```
composer require pouduo/iplocation

```

## use

```php
    use PouDuo\IpLocation\IpLocation;
```

## 示例用法
```php

   public function getArea(Request $request)
    {
        $IpLocation = new IpLocation();
        $area = $IpLocation->getlocation($request -> ip());
        return $area;
    }
```


