<fql output='table'>
  from
    NamingSystem
  where
    usage='Practitioner Identity'
  select
    uniqueId[0].value,
    name,
    description,
    responsible
  order by
    responsible
</fql>