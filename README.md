# tutorial-django-rest

Tutorial feito com objetivo de aprendizado profissional

* **Autor:** Wagner Esser
* **Tutorial:** [Django Rest Framework](http://www.django-rest-framework.org/tutorial/1-serialization/#tutorial-1-serialization).
* **Linguagem:** Python
* **Framework:** Django Rest

---
# Anotações do Tutorial

> *Serialização:* Em ciência da computação, no contexto de armazenamento e transmissão de dados, serialização é o processo de tradução de estruturas de dados ou estado de objeto em um formato que possa ser armazenado (por exemplo, em um arquivo ou buffer de memória, ou transmitido por meio de um enlace de conexão de rede) e reconstruído posteriormente no mesmo ou em outro ambiente computacional. [[Wikipédia](https://pt.wikipedia.org/wiki/Serializa%C3%A7%C3%A3o)].

* A classe *SnippetSerializer* em *serializers.py* comporta-se como um *Form* no Django.
    * `{'base_template': 'textarea.html'}` é equivalente à `widget=widgets.Textarea`.

