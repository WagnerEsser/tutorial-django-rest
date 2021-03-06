# tutorial-django-rest

Tutorial feito com objetivo de aprendizado profissional

* **Autor:** Wagner Esser
* **Tutorial:** [Django Rest Framework](http://www.django-rest-framework.org/tutorial/1-serialization/#tutorial-1-serialization).
* **Linguagem:** Python
* **Framework:** Django Rest

---
# Anotações do Tutorial

> **Serialização:** em ciência da computação, no contexto de armazenamento e transmissão de dados, serialização é o processo de tradução de estruturas de dados ou estado de objeto em um formato que possa ser armazenado (por exemplo, em um arquivo ou buffer de memória, ou transmitido por meio de um enlace de conexão de rede) e reconstruído posteriormente no mesmo ou em outro ambiente computacional. [[Wikipédia](https://pt.wikipedia.org/wiki/Serializa%C3%A7%C3%A3o)].

###### A classe *SnippetSerializer* em *serializers.py* comporta-se como um *Form* no Django.

`{'base_template': 'textarea.html'}` é equivalente à `widget=widgets.Textarea`.

###### Para testar, utilizar CURL ou HTTPIE ou Browser.
**HTTPIE:**

`pip install httpie`

Testar com:
```
http http://127.0.0.1:8000/snippets/ -a username
http http://127.0.0.1:8000/snippets/ Accept:application/json -a username
http http://127.0.0.1:8000/snippets/ Accept:text/html -a username
```

**CURL:**

Testar com:
```
curl -H 'Accept: application/json; indent=4' http http://127.0.0.1:8000/snippets/ -u username:senha
curl -H 'Accept: text/html; indent=4' http http://127.0.0.1:8000/snippets/ -u username:senha
```

Pode-se também alterar o cabeçalho `Content-type`:

```
http --form POST http://127.0.0.1:8000/snippets/ code="print 123" -a username
```

> **Mixins:** são classes prontas pensadas com foco no DRY.

> **DRY:** é um conceito de programação de computadores o qual propõe que cada porção de conhecimento em um sistema deve possuir uma representação única, de autoridade e livre de ambiguidades em todo o sistema. [[Wikipédia](https://en.wikipedia.org/wiki/Don't_repeat_yourself]