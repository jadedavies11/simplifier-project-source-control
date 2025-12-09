<fql output='table'>
  from
    NamingSystem
  where
    usage='Patient Identity'
  select
    usage,
    uniqueId[0].value,
    name,
    description,
    responsible
  order by
    responsible
</fql>