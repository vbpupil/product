# Base Product

## What?
Base product class which return the basis of what a product object is at its core.

## Why?
This class will form the absolute minimum for what a product is and should be used as the root to build more complex products on top.

## How?
```php
use vbpupil\Product\Product;

$ball = new Product('ball');
$ball
    ->setId(176)
    ->setDescription('intro','This ball is amazing!')
    ->setDescription('short','I am a short description.')
    
echo $ball->getName();
echo $ball->getId();
echo $ball->getDescription('intro');
echo $ball->getDescription('short');

$descriptions = $ball->getDescription(); //array of all descriptions returned
```