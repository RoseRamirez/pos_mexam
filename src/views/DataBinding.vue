<template>
<div class="container box-border h-100% w-100% m-auto mt-10 border-4 border-black bg-gray-200">
    <div class="m-10">
        <label class="text-xl font-bold text-black ">Customer Name: </label>
        <input type="text" v-model="fname">
    </div>


   <p class="text-4xl text-left font-bold text-black pl-32 ">RECEIPT</p>

   <h5>East Repair Inc.</h5>
   <h5>1912 Harvest Lane</h5>
   <h5>New Yok, NY 12210</h5>

   <h6 class="text-xl font-bold text-black">BILL TO:</h6>
   <h4>{{fname}}</h4>

<table class="rounded-t-lg m-5 w-5/6 mx-auto bg-gray-500 text-gray-800">
  <tr class="text-center border-b-2 border-gray-300 text-xl font-bold text-white">
    <th class="px-4 py-3">QTY</th>
    <th class="px-4 py-3">DESCRIPTION</th>
    <th class="px-4 py-3">UNIT PRICE</th>
    <th class="px-4 py-3">AMOUNT</th>
  </tr>
  
  <tr class="bg-gray-100 border-b border-gray-200 text-center">
    <td class="px-4 py-3"><input type="text" v-model="qty" /></td>
    <td class="px-4 py-3 font-semibold">Front and rear break cables</td>
    <td class="px-4 py-3"><input type="text" v-model="uprice" /></td>
    <td class="px-4 py-3">{{total}}</td>
  </tr> 

  <tr class="bg-gray-100 border-b border-gray-200 ">
    <td class="px-4 py-3"><input type="text" v-model="qty1" /></td>
    <td class="px-4 py-3 font-semibold">New set of pedal</td>
    <td class="px-4 py-3"><input type="text" v-model="uprice1" /></td>
    <td class="px-4 py-3">{{total1}}</td>
  </tr>

  <tr class="bg-gray-100 border-b border-gray-200">
    <td class="px-4 py-3"><input type="text" v-model="qty2" /></td>
    <td class="px-4 py-3 font-semibold">Labor 3 hours</td>
    <td class="px-4 py-3"><input type="text" v-model="uprice2" /></td>
    <td class="px-4 py-3">{{total2}}</td>
  </tr>

  <tr class="bg-gray-100 border-b border-gray-200">
    <td class="px-4 py-3"></td>
    <td class="px-4 py-3"></td>
    <td class="px-4 py-3 text-xl font-bold">TOTAL AMOUNT:</td>
    <td class="px-4 py-3 font-semibold">{{totaltotal}}</td>
  </tr>


</table>
</div>
</template>

<script>
    export default {
    name: 'Test',
    props: {
    msg: String
    },

    data(){
    return {
    fname: '',
    lname: '',
    qty: '',
    uprice: '',
    qty1: '',
    uprice1: '',
    qty2: '',
    uprice2: '',
    }
    },

    
    computed: 
    {
        total() {
        return parseInt(this.qty) * parseInt(this.uprice)
                },

                total1() {
        return parseInt(this.qty1) * parseInt(this.uprice1)
                },

                total2() {
        return parseInt(this.qty2) * parseInt(this.uprice2)
                },

                totaltotal() {
        return parseInt(this.total) + parseInt(this.total1) + parseInt(this.total2)
                }
    }
            
    }
    
</script>

<style scoped>
body{
     font-family: Verdana, Geneva, Tahoma, sans-serif;
}
h5{
     font-family: Verdana, Geneva, Tahoma, sans-serif;
    margin-top: 5px;
    text-align: left;
    padding-left: 10%;
    font-size: 15px;
}

h6{ 
     font-family: Verdana, Geneva, Tahoma, sans-serif;
    margin-top: 20px;
    text-align: left;
    padding-left: 10%;
    font-weight: bolder;
    font-size: 25px;
}

h4{ 
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    margin-top: 10px;
    text-align: left;
    padding-left: 10%;
    color: rgb(23, 23, 24);
    font-weight: bold;
    font-size: 20px;
}

</style>

