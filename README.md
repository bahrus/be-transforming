# be-transforming

```html
<form itemscope>
    <link itemprop=isHappy href=https://schema.org/True>
    <input type=checkbox name=isWealthy>
    <div contenteditable id=liberated>abc</div>
    ...
    <div itemscope
        onload="
        {
            prop1: isHappy && !isWealthy && liberated?.length > 17,
            prop2: liberated?.blink()
        }
        " 
        be-computed='from $isHappy, @isWealthy, #liberated, and assign result to scope.'
        be-transforming='of $0:bE:scoped' data-xform='{
            "span": "prop1",
            "section": "prop2"
        }'>
        <span></span>
        <section></section>
    </div>
</form>
```
