# Header 1
text 1.
## Header 2
text 2.
### Header 3
text 3.

![01_1](./images/01.png)

```mermaid
graph LR
    A[Первый блок] --> B[Второй блок]
```

<!-- Client-side Mermaid renderer -->
<script src="https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.min.js"></script>
<script>
document.addEventListener('DOMContentLoaded', function(){
    document.querySelectorAll('pre > code.language-mermaid, code.language-mermaid').forEach(function(el){
        var pre = el.parentElement;
        var wrapper = document.createElement('div');
        wrapper.className = 'mermaid';
        wrapper.textContent = el.textContent;
        pre.parentNode.replaceChild(wrapper, pre);
    });
    if (typeof mermaid !== 'undefined') {
        mermaid.initialize({ startOnLoad: true });
    }
});
</script>
