# User Module für ZF2

Dies wird ein UserModul für ZF2.

Bisher gibt es im Controoler nur folgende Aktionen:

  - Index (indexAction)
  - Anmelden (loginAction)
  - Registrieren (registerAction)

Von [Andreas Vogelbacher] für ein Semesterprojekt in der [ABB-TS] [1]:

#### <i class="icon-pencil"></i> Version
0.0.1

> Achtung:
> Early beta

### Installation

```sh
$ composer update
```


.....

> Es kommen ein paar Markdown Tests um rauszufinde wie das Funktioniert:
## Mardown Tests

### Footnotes

You can create footnotes like this[^footnote].

  [^footnote]: Here is the *text* of the **footnote**.
  
### MathJax

You can render *LaTeX* mathematical expressions using **MathJax**, as on [math.stackexchange.com][1]:

The *Gamma function* satisfying $\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$ is via the Euler integral

$$
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
$$


### UML diagrams

You can also render sequence diagrams like this:

```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
```

And flow charts like this:

```flow
st=>start: Start
e=>end
op=>operation: My Operation
cond=>condition: Yes or No?

st->op->cond
cond(yes)->e
cond(no)->op
```

```
<script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS_HTML"></script>
```

```javascript
$(function(){
  $('div').html('I am a div.');
});
```

```php
public function registerAction()
    {
        $view = new ViewModel();
        $view->setTemplate('users/index/new-user');
        return $view;
    }
```


[Andreas Vogelbacher]:nixda@willkeinspam.com
[1]:http://abbts.ch
