<fql output='table'>
  from
    NamingSystem
  where
    usage='Document identity'
  select
    uniqueId[0].value,
    name,
    description,
    responsible
  order by
    responsible
</fql>