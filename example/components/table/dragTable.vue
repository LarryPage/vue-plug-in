<template>
  <div class="dragTable">

    <table class="table table-condensed">
      <caption>编排工序</caption>
      <thead>
      <tr>
        <th>名称1</th>
        <th>名称2</th>
        <th>名称3</th>
        <th>名称4</th>
        <th>名称5</th>
        <th>名称6</th>
      </tr>
      </thead>
      <td-draggable  class="list-group" v-model="list"  :options="dragOptions" element="tbody" tag="tbody" @start="startDrag" @end="onEndDrag" >
          <tr  v-for="(item,index) in list" class="item" :key="'item'+index">
            <td>{{item.complete}}</td>
            <td>{{item.code}}</td>
            <td>{{item.name}}</td>
            <td>{{item.time}}</td>
            <td>{{item.person}}</td>
            <td>{{item.stations}}</td>
          </tr>
      </td-draggable>
    </table>

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      dragOptions: {
        draggable: '.item'
      },
      list: [{
        complete: '1',
        code: 'no',
        name: '盘点单号12323',
        time: 111,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '2',
        code: 'no',
        name: '盘点单号2222',
        time: 3333,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '3',
        code: 'no',
        name: '盘点单号22215235',
        time: 324234,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '4',
        code: 'no',
        name: '盘点单号232423432',
        time: 235325,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '5',
        code: 'no',
        name: '盘点单号24324324',
        time: 32341,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '6',
        code: 'no',
        name: '盘点单号2324234',
        time: 123123,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }, {
        complete: '7',
        code: 'no',
        name: '盘点单号3324',
        time: 8567567,
        person: '泥工',
        stations: 'xx'
      }]
    }
  },
  components: {
  },
  methods: {
    onEnd () {
      console.log(this.list)
    },
    startDrag (data) {
      console.log(data)
    },
    onEndDrag (data) {
      console.log(data)
    }
  }
}
</script>
<style scoped>

</style>
