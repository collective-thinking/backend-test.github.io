# PHP

## 1. What is the size of this array? 
```php
$arr = []; 
$arr[8] = 'test';
```

**Answer:** 
  - [ ] 1 
  - [ ] 8 
  - [ ] 9


## 2. How many classes are instantiated?
```php
class A { }
class B { }
              
$a = new A(); 
$b = new B();
$c = $b;
```

**Answer:**
  - [ ] 1
  - [ ] 2
  - [ ] 3

## 3. What is are the output of the following snippets?

A.
```php 
$arr = [3, 0];
foreach ($arr as $item) {
    $item++;
}
$nb = (int) implode('', $arr);
echo $nb;
```

**Answer:**

B.
```php
$a = '1';
$b = &$a;
$b = "4{$b}";
echo $a . ',' . $b++;
```

**Answer:**

## 4. Which PHP code snippet shows an example of Dependency Injection?

A.
```php
class Client 
{
    private $logger;
    
    public function __construct(LoggerInterface $logger)
    {
        $this->logger = $logger;
    }
}
```

B.
```php
class Client 
{
    private $logger;
    
    public function __construct()
    {
        $this->logger = new Logger();
    }
}
```

C.
```php
    $client = new Client();
    $logger = new Logger();
    inject($client, $logger);
```

**Answer:**
  - [ ] A
  - [ ] B
  - [ ] C


## 5. Name the following design patterns.

#### Design Pattern #1

```php
class MyClass 
{
    public static function newInstance(string: $type): Formatter {
        if ('number' === $type) {
            return new FormatNumber();
        } elseif ('string' === $type) {
            return new FormatString();
        }
    }
}
```
   
**Answer** : ?
   
#### Design Pattern #2   

```php
class MyClass 
{
    private $_stays = [];

    private $_currentIndex = 0;

    public function count(): int
    {
        return count($this->_stays);
    }

    public function current(): Stay
    {
        return $this->_stays[$this->_currentIndex];
    }

    public function key: int
    {
        return $this->_currentIndex;
    }

    public function next()
    {
        return $this->_currentIndex++;
    }

    public function rewind()
    {
        return $this->_currentIndex = 0;
    }

    public function valid(): bool
    {
        return isset($this->_stays[$this->_currentIndex]);
    }
}
```

**Answer** : ?

