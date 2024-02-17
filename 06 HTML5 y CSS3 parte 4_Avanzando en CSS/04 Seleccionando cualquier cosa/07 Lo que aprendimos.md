Lo que aprendimos en esta aula:

Selectores avanzados CSS

- Selector `>` , para acceder a los hijos de determinado elemento. Por ejemplo, para acceder todos los `p` dentro del `main`:

```css
main > p {          }
```

- Selector `+`, para acceder al primer hermano de determinado elemento. Por ejemplo, para acceder el primer `p` después de una `img`:

```css
img + p {
}
```

- Selector `~`, para acceder a todos los hermanos de determinado elemento. Por ejemplo, para acceder todos los `p` después de una `img`:

```css
img ~ p {
}
```

- Selector `not`, para acceder a los elementos, excepto algunos. Por ejemplo, para acceder a todos los `p` dentro de `main` excepto el `p` que tiene `id` `mission`:

```css
main p:not(#mission) {
}
```

- Cómo hacer cuentas con CSS, con la propiedad `calc`