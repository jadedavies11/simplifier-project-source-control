<fql output='table'>
  from
    NamingSystem
  where
    responsible.contains(%responsiblename)
  select
    UID: uniqueId[0].value,
    Name: name,
    Purpose: usage,
    Details: description
  order by
    usage
</fql>