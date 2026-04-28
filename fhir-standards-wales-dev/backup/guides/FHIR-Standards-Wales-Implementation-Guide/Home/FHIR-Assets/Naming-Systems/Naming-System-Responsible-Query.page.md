<fql output='table'>
  from
    NamingSystem
  where
    responsible.contains(%responsiblename)
  select
    uniqueId[0].value,
    name,
    usage,
    description
  order by
    usage
</fql>