<script src="//unpkg.com/vue/dist/vue.js"></script>
<script src="//unpkg.com/element-ui@2.3.9/lib/index.js"></script>

<template>
  <div class="el-table__header">
    <el-table
      :data="tableData"
      :row-style="tableRowStyle"
      :cell-style="tableColor"
      border
      style="width: 100%"
      :row-class-name="tableRowClassName"
      
    >
      <el-table-column
        prop="tarih"
        class="el-icon-error"
        label="Tarih"
        width="190px"
      >
      </el-table-column>
      <el-table-column prop="ıd" label="ID" sortable width="190px">
      </el-table-column>
      <el-table-column prop="kurum" label="Kurum" width="190px">
      </el-table-column>
      <el-table-column prop="kategori" sortable label="Kategori" width="180px">
      </el-table-column>
      <el-table-column
        prop="uçuş"
        sortable
        label="Uçuş Saatleri US"
        width="190px"
      >
      </el-table-column>
      <el-table-column prop="kuyruk" label="Kuyruk No." width="190px">
      </el-table-column>
      <el-table-column prop="ucus" label="Uçuş No." width="190px">
      </el-table-column>
      <el-table-column prop="pax" label="PAX" width="186px"> </el-table-column>
    </el-table>
  </div>
</template>

<script>
export default {
  name: "table",
  data() {
    return {
      tableData: [
        {
          tarih: "",
          ıd: "2",
          kurum: <div style="backround='#red' ">CRNDN</div>,
          kategori: "HAVAYOLU 1",
          uçuş: "",
          kuyruk: "",
          ucus: "",
          pax: "0",
        },
        {
          tarih: "",
          ıd: "3",
          kurum: "CRNDN",
          kategori: "HAVAYOLU 1",
          uçuş: "",
          kuyruk: "",
          ucus: "",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "4",
          kurum: "CRNDN",
          kategori: "HAVAYOLU 1",
          uçuş: "",
          kuyruk: "",
          ucus: "",
          pax: "0",
        },
        {
          tarih: "",
          ıd: "5",
          kurum: "CRNDN",
          kategori: "HAVAYOLU 1",
          uçuş: "",
          kuyruk: "",
          ucus: "",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "6",
          kurum: "CRNDN",
          kategori: "HAVAYOLU 1",
          uçuş: "",
          kuyruk: "",
          ucus: "",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "7",
          kurum: "KOZ",
          kategori: "HAVAYOLU 2",
          uçuş: <span class="el-icon-alarm-clock"></span>,
          kuyruk: "TC-CON",
          ucus: "CAI901P",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "8",
          kurum: "KOZ",
          kategori: "HAVAYOLU 2",
          uçuş: <span class="el-icon-alarm-clock"></span>,
          kuyruk: "TC-TJS",
          ucus: "CAI194P",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "9",
          kurum: "KOZ",
          kategori: "HAVAYOLU 1",
          uçuş: "",
          kuyruk: "",
          ucus: "",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "10",
          kurum: "KOZ",
          kategori: "HAVAYOLU 1",
          uçuş: "",
          kuyruk: "",
          ucus: "",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "11",
          kurum: "KOZ",
          kategori: "HAVAYOLU 2",
          uçuş: <span class="el-icon-alarm-clock"></span>,
          kuyruk: "TC-TJS",
          ucus: "CAI197P",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "13",
          kurum: "CRNDN",
          kategori: "HAVAYOLU 2",
          uçuş: <span class="el-icon-alarm-clock"></span>,
          kuyruk: "",
          ucus: "ACG97HY",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "14",
          kurum: "CRNDN",
          kategori: "HAVAYOLU 2",
          uçuş: <span class="el-icon-alarm-clock"></span>,
          kuyruk: "",
          ucus: "ACG97HY",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "15",
          kurum: "KOZ",
          kategori: "HAVAYOLU 2",
          uçuş: <span class="el-icon-alarm-clock"></span>,
          kuyruk: "TC-TJS",
          ucus: "CAI1966",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "16",
          kurum: "KOZ",
          kategori: "HAVAYOLU 2",
          uçuş: <span class="el-icon-alarm-clock"></span>,
          kuyruk: "TC-TJS",
          ucus: "CAI1966",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "17",
          kurum: "CRNDN",
          kategori: "HAVAYOLU 1",
          uçuş: "",
          kuyruk: "",
          ucus: "",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "18",
          kurum: "PEGAS",
          kategori: "KPEGAS-TİP1",
          uçuş: <span class="el-icon-alarm-clock"></span>,
          kuyruk: "35RTV53V",
          ucus: "34FLGHT67",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "19",
          kurum: "KOZ",
          kategori: "HAVAYOLU 2",
          uçuş: <span class="el-icon-alarm-clock"></span>,
          kuyruk: "TC-TJN",
          ucus: "CAI555",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "20",
          kurum: "PEGAS",
          kategori: "DENEME TİP 1",
          uçuş: <span class="el-icon-alarm-clock"></span>,
          kuyruk: "35TAJL35",
          ucus: "",
          pax: "0",
        },
        {
          dtarih: "",
          ıd: "21",
          kurum: "CRNDN",
          kategori: "HAVAYOLU 1",
          uçuş: "",
          kuyruk: "",
          ucus: "35FLIGHT35",
          pax: "0",
        },
      ],
    };
  },
  created() {},
  methods: {
    tableRowStyle({ row, rowIndex }) {
      return "background-color: pink";
    },
    //  modify the table header the background color
    tableColor({ row, column, rowIndex, columnIndex }) {
      if (rowIndex === 0 && columnIndex === 2) {
        return "background-color: #2CD5C4;";
      }
      if (rowIndex === 1 && columnIndex === 2) {
        return "background-color: #2CD5C4;";
      }
      if (rowIndex === 2 && columnIndex === 2) {
        return "background-color: #2CD5C4;";
      }
      if (rowIndex === 3 && columnIndex === 2) {
        return "background-color: #2CD5C4;";
      }
      if (rowIndex === 4 && columnIndex === 2) {
        return "background-color: #2CD5C4;";
      }
      if (rowIndex === 5 && columnIndex === 2) {
        return "background-color: #AED000;";
      }
      if (rowIndex === 6 && columnIndex === 2) {
        return "background-color: #AED000;";
      }
      if (rowIndex === 7 && columnIndex === 2) {
        return "background-color: #AED000;";
      }
      if (rowIndex === 8 && columnIndex === 2) {
        return "background-color: #AED000;";
      }
      if (rowIndex === 9 && columnIndex === 2) {
        return "background-color: #AED000;";
      }
      if (rowIndex === 10 && columnIndex === 2) {
        return "background-color: #2CD5C4;";
      }
      if (rowIndex === 11 && columnIndex === 2) {
        return "background-color: #2CD5C4;";
      }
      if (rowIndex === 12 && columnIndex === 2) {
        return "background-color: #AED000;";
      }
      if (rowIndex === 13 && columnIndex === 2) {
        return "background-color: #AED000;";
      }
      if (rowIndex === 14 && columnIndex === 2) {
        return "background-color: #2CD5C4;";
      }
      if (rowIndex === 15 && columnIndex === 2) {
        return "background-color: #C1A7E2;";
      }
      if (rowIndex === 16 && columnIndex === 2) {
        return "background-color: #AED000;";
      }
      if (rowIndex === 17 && columnIndex === 2) {
        return "background-color: #C1A7E2;";
      }
      if (rowIndex === 18 && columnIndex === 2) {
        return "background-color: #2CD5C4;";
      }
      if (rowIndex === 15 && columnIndex === 3) {
        return "background-color: #F3D03E;";
      }
      if (rowIndex === 17 && columnIndex === 3) {
        return "background-color: #279989;";
      }
    },
    renderheader(h, { column }) {
      //h is short for cerateelement, please refer to the official vue documentation
      return h("div", [
        h("span", column.label),
        h("i", {
          class: "el-icon-error",
          style: "color:#409eff;margin-left:5px;",
        }),
      ]);
    },
  },
};
</script>
var Ctor = Vue.extend(Main)
new Ctor().$mount('#app')

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.el-table .warning-row {
  background: oldlace;
}

.el-table .success-row {
  background: #f0f9eb;
}
</style>
