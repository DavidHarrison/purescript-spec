## Module Test.Spec.Reporter

#### `Entry`

``` purescript
data Entry
  = Describe (Array Name)
  | It Name Result
  | Pending Name
```

##### Instances
``` purescript
instance eqEntry :: Eq Entry
instance showEntry :: Show Entry
```

#### `Reporter`

``` purescript
type Reporter e = Array Group -> Eff e Unit
```

#### `collapse`

``` purescript
collapse :: Group -> Array Entry
```


