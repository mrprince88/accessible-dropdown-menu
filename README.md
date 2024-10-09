## Accessible Dropdown Menu

Introducing a hook to create an accessible dropdown easily in few steps. This hook handles all the accessibility logic when building a dropdown menu, dropdown button, etc., and leaves the design completely up to you.

- Fully accessible with keyboard and mouse navigations.
- Zero dependencies

# Usage

Import the hook:

``` 
import useDropdown from accessible-dropdown-menu
```

Use the hook:

```  
const { buttonProps, itemProps, isOpen, setIsOpen } = useDropdownMenu<HTMLDivElement>(numberOfItems, currSelectedValue);
```

For button that triggers the dropdown:

```
<button
  {...buttonProps}
>
```

For options in the list:

```
<li
  key={option}
  {...itemProps[index]}
  >
  {name}
</li>
```
