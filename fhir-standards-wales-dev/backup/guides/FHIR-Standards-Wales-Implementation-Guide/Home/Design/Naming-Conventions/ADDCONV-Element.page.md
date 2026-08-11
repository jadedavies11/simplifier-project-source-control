<span style="font-size: 0.9em;">The fields within a profile that store information are called elements. Any core element name is unchangeable and is dictated by HL7 and UK Core depending on who created the element. We can however create our own elements as extensions and slices. In all cases elements use the [lowerCamelCase](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case) naming convention. e.g. DocumentReference.extension:digitalStatus</span><br />

<span style="font-size: 0.9em;">In the special case where a backport extension is used from a later FHIR release, the slice name for the extension is suffixed by the release number e.g. DocumentReference.extension:versionR5​</span>

