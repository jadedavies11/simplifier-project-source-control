<fql output='table'>
  from
    NamingSystem
  where
    usage='Organization Identity'
  select
    uniqueId[0].value,
    name,
    description,
    responsible
  order by
    responsible
</fql>