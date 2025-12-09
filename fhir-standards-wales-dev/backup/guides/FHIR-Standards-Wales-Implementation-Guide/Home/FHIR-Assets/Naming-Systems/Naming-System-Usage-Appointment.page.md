<fql output='table'>
from
  NamingSystem
where
  responsible='Aneurin Bevan University Health Board'
select
  uniqueId[0].value,
  name,
  description,
  usage
order by
  usage
</fql>
