//partes do elemento
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX : <http://www.daml.org/2003/01/periodictable/PeriodicTable#>
select DISTINCT ?types where{
    ?s owl:onProperty ?types.
}

//partes do grupo
PREFIX : <http://www.daml.org/2003/01/periodictable/PeriodicTable#>
select DISTINCT ?types where{
    ?s a :Group.
    ?s ?types ?r.
}