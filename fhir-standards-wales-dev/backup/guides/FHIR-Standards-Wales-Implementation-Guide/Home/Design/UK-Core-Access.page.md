---
canonical: 'https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Organization'
---
# {{page-title}}

## Overview
<fql output="inline">
	from
		StructureDefinition
	where
		url = %canonical
	select
		description
</fql>

## Metadata
<fql output="table">
	from
		StructureDefinition
	where
		url = %canonical
	select
		Name: name,
		Canonical_URL: url,
		Status: status,
		Version: version
</fql>

### Formal Views of Profile Content
<tabs>
<tab title="Overview">
	{{tree, buttons}}
</tab>
<tab title="Detailed View">
	{{dict}}
</tab>
<tab title="XML">
	{{xml}}
</tab>
<tab title="JSON">	
	{{json}}
</tab>
<tab title="Link">
	{{link}}
</tab>
</tabs>

### Differentials
#### Must Support Elements
<fql>
	from
    	StructureDefinition
	where
    	url = %canonical
	select
    	join for differential.element
      		select {
				Path: id,
				join
				for mustSupport
				select {
					Must_Support: true}
        	}
</fql>

#### Slices
<fql>
	from
    	StructureDefinition
	where
    	url = %canonical
	select
    	join for differential.element
      		select {
				Path: id,
				join
				for slicing
				where discriminator.exists()
				select {
					Type: type,
					Path: path}
        	}
</fql>

#### Terminology Bindings
<fql>
	from
    	StructureDefinition
	where
    	url = %canonical
	select
    	join for differential.element
      		select {
				Path: id,
				join
				for binding
				where valueSet.exists()
				select {
					Conformance: strength,
					ValueSet: valueSet}
        	}
</fql>

#### Extensions
<fql>
	from
    	StructureDefinition
	where
    	url = %canonical
	select
    	join for differential.element
      		select {
				Path: id,
				join
				for type
				where path.contains(extension)
				select {
					Path: path,
					Extension: profile}
        	}
</fql>

#### Constraints
<fql>
  from
		StructureDefinition
  where
		url = %canonical
  select
		differential.element {
			Path: id,
			join constraint {
				Id: key,
				Grade: severity,
				Details: human
				}
			}
</fql>

### Examples

### Guidance Categories
