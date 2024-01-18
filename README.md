Suppose you have a Discourse group, "supporters". (This could be a group where membership is based on the user having a paying subscription.)

## Quick template copy-and-paste

```
<div data-umbgrsw="supporters">
</div>

<div data-umbgrsw="%!supporters">
</div>
```

## Group-based switching

```
This is text everyone would see.

<div data-umbgrsw="supporters">
Only show this enclosed content if the user is a member of the *supporters* group.
</div>

Also text everyone would see.

<div data-umbgrsw="!supporters">
Only show this enclosed content if the user is NOT a member of the *supporters* group.
</div>

Still more text everyone would see.
```

## Displaying the default content

The default content—configured in the component's settings—will be inlined if the specification for displaying the enclosed content starts with a % character.

Below, for users not in the group, they would see the default content in place of the DIV.
```
<div data-umbgrsw="%!supporters"></div>
```

Below, for users in the group, they would see the default content in place of the DIV.
```
<div data-umbgrsw="%foogroup"></div>
```

