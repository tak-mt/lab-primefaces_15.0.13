# idim-theme

Reusable PrimeFaces custom theme module for the iDIM team.

The module now owns the Azure Portal-derived Sass source and compiles its packaged theme during the Maven build.

## Coordinates

- `groupId`: `com.idim.primefaces`
- `artifactId`: `idim-theme`
- `version`: `1.01a-SNAPSHOT`

## Packaged Theme Name

- `idim-theme`

PrimeFaces should resolve the theme from:

- `META-INF/resources/primefaces-idim-theme/theme.css`

Editable source lives under:

- `src/main/sass/primefaces-idim-theme`

## Build

```sh
mvn clean package
```

The generated artifact will be:

```text
target/idim-theme-1.01a-SNAPSHOT.jar
```

## Use In Another Application

Add the dependency:

```xml
<dependency>
    <groupId>com.idim.primefaces</groupId>
    <artifactId>idim-theme</artifactId>
    <version>1.01a-SNAPSHOT</version>
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

- The Azure Portal theme source has been relocated into this module from the checked-out PrimeFaces sources.
- Update the Sass files in `src/main/sass/primefaces-idim-theme` when changing shared team branding.
