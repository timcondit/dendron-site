---
id: 99f7dd68-b2dc-46d0-a556-8a607223dc25
title: Lookup
desc: ''
updated: 1604600828175
created: 1602392064100
stub: false
---

# Lookup

## Lookup Command

- src: plugin-core/src/components/lookup/LookupControllerV2.ts

```ts
show {
    ...
    provider = new LookupProviderV2
    picker :=

    @updatePickerBehavior(provider, picker)
    quickPick.onDidTriggerButton = ...
    ...
    provider.provide(quickPick)
    ...
    quickPick.show
}
```

### updatePickerBehavior
```ts
updatePickerBehavior(quickpick, provider) {
    buttons := 
    selectedPath := buttons
    selectedSelection := buttons

    switch selectedPath {
        case journal {
            quickpick.value := 
            provider.onUpdatePickerItem(
                ....
            )
        }
    }

    switch selectedSelection {
        case {
            ...
        }
    }

}
```

### provide
- file: src/components/lookup/LookupProviderV2.ts

```ts
provider picker {
    picker.onDidAccept = @onDidAccept
    picker.onDidChangeValue = @onUpdatePickerItem
}

```

## Lookup Modifiers

```ts
cons(opts) {
    lookupSelectionType := CONFIG.DEFAULT_LOOKUP_CREATE_BEHAVIOR
    noteSelectionType := opts
    effectTypes := opts

    types = [lookupSelectionType, noteSelectioType, effectTypes]

    this.state {
        buttons: createAllButtons(types)
    }
}

show {
    picker := createPicker
    ...
    @updatePickerBehavior(picker)
    @refreshButtons(picker, @state.buttons)
    picker.onTriggerButton = @onTriggerButton

}

onTriggerButton(btn) {
    btnTriggered := find(state.buttons, btn)
    btnTriggered.pressed = !btnTriggered.pressed
    btnCategory := btn
    ...
    @refreshButtons(picker, @state.buttons)
    @updatePickerBehavior
}

updatePickerBehavior {
    ...
    @updateBehaviorByEffect
    @updateBehaviorByNoteType

}
updateBehaviorByEffect {
    effectButtons.map(btn.handle)
}

updateBehaviorByNoteType {
    ...
    provider.onUpdatePickerItem(quickPick, provider.opts, onUpdateReason);
}
```


```ts
onUpdatePickerItem(picker) {

    showRootResults if (qs == "")

    updatedItems = picker.items


    if (qs.endsWith(.) || query.levels < 2 || picker.justActivated) {
        resp = engine.query
        updatedItems = [noActiveItem] + resp
    }

    ...

    addSchemaSuggestions(qs)


}

```