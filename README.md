CSS - Cascading Style Sheet  (Cascading - multiple rules and properties can be applied to elements)

Inline Styles > Id Selectors #id > Class Selectors .demo and Attribute Selectors [disabled] > Tag Selector h1, h2

==================================================================================================================

COMBINATORS

Adjacent Sibling (element should be direct sibling)

div + h1 {
    color: red;                      
}

<div>demo</div>
<h1>It will be in red<h1>
<div>demo</div>
<h1>It will be in red<h1>
<span>demo</span>
<h1>It will not be in red<h1>



General Sibling (element need not to be direct sibling)

div ~ h1 {
    color: red;                      
}

<div>demo</div>
<h1>It will be in red<h1>
<div>demo</div>
<h1>It will be in red<h1>
<span>demo</span>
<h1>It will be in red<h1>



Child Combinators (element need to be child of element)

div > h1 {
    color: red
}

<div>
    demo
    <h1>it will be in red</h1>
    <span>
      <h1>it will be not red</h1>
    </span>
</div>


Descendant Combinators (element can be of same level or child)

div h1 {
    color: red
}

<div>
    demo
    <h1>it will be in red</h1>
    <span>
      <h1>it will be in red</h1>
    </span>
</div>

==================================================================================================================

BOX MODEL

+------------------------------+
|          Margin              |
|  +------------------------+  |
|  |        Border          |  |
|  |  +------------------+  |  |
|  |  |     Padding      |  |  |
|  |  |  +------------+  |  |  |
|  |  |  |  Content   |  |  |  |
|  |  |  +------------+  |  |  |
|  |  +------------------+  |  |
|  +------------------------+  |
+------------------------------+



