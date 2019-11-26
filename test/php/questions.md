
# PHP

## 1. Quelle est la taille du tableau ci-dessous ? 
<pre>
$arr = []; 
$arr[8] = 'test';
</pre>                
Réponse : 1 / 8 / 9


## 2. Instance de classe

Combien de classe ont été instanciées ?
<pre>
class A { }
              
$a = new A(); 
$b = new B();
$c = $b;
</pre>
Réponse : 1 / 2 / 3


## 3. Design pattern

Quel sont les noms des design pattern suivants ?
<pre>
class MyClass 
{
    public static function  new Instance(string: $type): Formatter {
        if ('number' === $type) {
            return new FormatNumber();
        } elseif ('string' === $type) {
            return new FormatString();
        }
    }
}
</pre>

<pre>
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
</pre>