
# Creating your travel list
1. Choose the number of days
2. You choose a number of presets. f.ex Summer, Winter, Medicine, Makup, etc...
3. Add additional items
4. Start packing - cross items off
5. Share lists with <3

Different types of lists:
- Sharing a list
    + Data is shared and updated across parties
    + Can see items as packed (by whom)
- Copying a list
    + List is copied and updated individually

## Category definition
```
{
    name: 'summer (women)',
    items: [{...}]
}
```

## Item definition
```
[{
    name: 'underware',
    definition: {
        type: 'multipler',
        factor: 2
    },
    packed: false
}, {
    name: 'sun glasses',
    definition: {
        type: 'static'
    },
    packed: false
}]
```

### Item type def
- Multiplier items (multiply per day factor)
    + Per day factor
- Static item (you take these as is)

## Packing list
- Add any other items to the `other` category
```
{
    name: 'Panama holiday',
    days: 8,
    categories: [{...}, {
        name: 'other',
        items: [{...}]
    }]
}
```
