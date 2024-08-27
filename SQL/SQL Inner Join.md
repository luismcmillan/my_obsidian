[[SQL]]
```SQL
select c.id, c.name, c.schnauze from zoo.raubtier c
inner join zoo.wolf w on w.alter = c.alter 
```