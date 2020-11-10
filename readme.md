# dataspice-example

Example repo to show off [dataspice](https://github.com/ropenscilabs/dataspice).

```r
library(dataspice)

create_spice() # Creates metadata templates for us
write_spice() # Creates a JSON-LD document from our metadata
build_site() # Creates a web page from our JSON-LD

# Optionally, convert to EML
eml <- spice_to_eml()

# Validation will show errors after conversion because EML is much richer than
# dataspice/Schema.org so some information will be missing and need to be filled
# in after conversion
EML::eml_validate(eml)
```

