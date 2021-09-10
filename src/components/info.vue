<template>

<table id="info" width="400px" max-height="300px">
<caption>DMU-65</caption>
<tr>
  <th>id</th>
  <th>Название</th>
  <th>Информация</th>
</tr>
<tr v-for="item in kontroledParams" :key="item.id">
  <td>{{item.id}}</td>
  <td>{{item.name}}</td>
  <td>{{item.information}}</td>
</tr>
</table>
</template>

<script>
export default {
data(){
  return{
  kontroledParams:[
    {id:1,name: 'Неисправный элемент', information:'Подшипник 2 Х 466880' },
    {id:2,name: 'Характеристики',information:'радиально-упорный шарикоподшипник, однорядный, для спаренного монтажа'},
    {id:3,name: 'Производство',information:'SKF'},
    {id:4,name: 'Аномальный контрольный параметр',information:'Виброскорость=6.5 м/с (в допуске <4.2м/с)' },
    {id:5,name: 'Вид ремонта',information:'Замена'},
    {id:6,name: 'Срочность ремонта',information:'неотложная' }
  ]
  }
}
}
</script>

<style>
table{
  max-height: 300px;
}
th{
  border: 2px solid lightgray;
}
tr{
border: 2px solid black;
}
td{
  border: 1px solid gray;
  align-items: center;
  
}
</style>  
