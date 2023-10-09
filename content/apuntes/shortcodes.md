+++
title = 'Shortcodes'
date = 2023-09-25T10:08:10+02:00
+++

Hugo utiliza Markdown por su formato de contenido simple. Sin embargo, hay muchas cosas que Markdown no admite bien. Podría utilizar HTML puro para ampliar las posibilidades.

Pero resulta que esto es una mala idea. Todo el mundo usa Markdown porque es puro y simple de leer incluso sin renderizar. Debes evitar HTML para mantenerlo lo más simple posible.

Para evitar estas limitaciones, Hugo creó shortcuts. Un shortcode es un fragmento simple dentro de una página.

### 1. Attachments

El attachments shortcode muestra una lista de archivos adjuntos a una página con color, título e icono ajustables.

{{% attachments sort="asc" style="warning" /%}}
{{% attachments  sort="asc" style="tip" /%}} 
{{% attachments  sort="asc" style="note" /%}}
{{% attachments  sort="asc" style="info" /%}}


### 2. Badge

El badgeshortcode muestra pequeños marcadores en su texto con color, título e ícono ajustables.

{{% badge %}}Important{{% /badge %}}
{{% badge style="primary" title="Version" %}}6.6.6{{% /badge %}}
{{% badge style="red" icon="angle-double-up" %}}Captain{{% /badge %}}
{{% badge style="info" %}}New{{% /badge %}}
{{% badge color="fuchsia" icon="fab fa-hackerrank" %}}Awesome{{% /badge %}}


### 3. Button

El button shortcut muestra un botón en el que se puede hacer clic con color, título e icono ajustables.

{{% button href="https://gohugo.io/" %}}Get Hugo{{% /button %}}
{{% button href="https://gohugo.io/" style="warning" icon="dragon" %}}Get Hugo{{% /button %}}
{{% button href="https://gohugo.io/" icon="download" %}}Get Hugo{{% /button %}}

<form action="../../search.html" method="get">
  <input name="search-by-detail" class="search-by" type="search">
  {{% button type="submit" style="secondary" icon="search" %}}Search{{% /button %}}
</form>

### 4. Children
### 5. Expand

{{% expand "Expand me..." %}}Thank you!{{% /expand %}}

### 6. Highlingt

{{< highlight lineNos="true" type="py" wrap="true" title="python" >}}
print("Hello World!")
{{< /highlight >}}

### 7. Icon

{{% icon icon="exclamation-triangle" %}}
{{% icon icon="angle-double-up" %}}
{{% icon icon="skull-crossbones" %}}


### 9. Math

{{< math align="center" >}}
$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$
{{< /math >}}

### 10. Mermaid

{{< mermaid align="center" zoom="true" >}}
graph LR;
    If --> Then
    Then --> Else
{{< /mermaid >}}

### 11. SiteParam

`editURL` value: {{% siteparam name="editURL" %}}

### 12. Tab
{{% tab title="c" %}}
```c
printf("Hello World!");
```
{{% /tab %}}

### 13. Tabs

{{< tabs title="hello." >}}
{{% tab title="py" %}}
```python
print("Hello World!")
```
{{% /tab %}}
{{% tab title="sh" %}}
```bash
echo "Hello World!"
```
{{% /tab %}}
{{% tab title="c" %}}
```c
printf"Hello World!");
```
{{% /tab %}}
{{< /tabs >}}