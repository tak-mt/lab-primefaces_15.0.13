# idim-theme

Reusable PrimeFaces custom theme module for the iDIM team.

## Coordinates

- `groupId`: `com.idim.primefaces`
- `artifactId`: `idim-theme`
- `version`: `101a`

## Packaged Theme Name

- `idim-theme`

PrimeFaces should resolve the theme from:

- `META-INF/resources/idim-theme/theme.css`

## Build

```sh
mvn clean package
```

The generated artifact will be:

```text
target/idim-theme-101a.jar
```

## Use In Another Application

Add the dependency:

```xml
<dependency>
    <groupId>com.idim.primefaces</groupId>
    <artifactId>idim-theme</artifactId>
    <version>101a</version>
</dependency>
```

Then set the PrimeFaces theme:

```xml
<context-param>
    <param-name>primefaces.THEME</param-name>
    <param-value>idim-theme</param-value>
</context-param>
```

## Notes

- This module is currently seeded from the Azure Portal style theme in the checked-out PrimeFaces sources.
- Keep shared team branding changes inside `src/main/resources/META-INF/resources/idim-theme/theme.css`.
