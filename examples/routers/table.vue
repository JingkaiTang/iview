<template>
    <div>
        <div style="width: 550px;">
            <Table height="200" border :columns="columns2" :data="data4"></Table>
        </div>
        <br><br><br>
        <Table width="550" height="200" border :columns="columns2" :data="data4"></Table>
        <br><br><br>
        <Table :columns="columns3" :data="data3"></Table>
    </div>
</template>
<script>
    export default {
        data () {
            return {
                columns3: [
                    {
                        width: 80,
                        title: '#',
                        type: 'index'
                    },
                    {
                        width: 80,
                        type: 'selection'
                    },
                    {
                        minWidth: 120,
                        title: 'Column 1',
                        key: 'c1'
                    },
                    {
                        minWidth: 120,
                        title: 'Column 2',
                        key: 'c2'
                    },
                    {
                        maxWidth: 300,
                        minWidth: 100,
                        title: 'Column 3',
                        key: 'c3'
                    },
                    {
                        minWidth: 300,
                        title: 'Column 4',
                        key: 'c4'
                    },
                    {
                        minWidth: 100,
                        title: 'Column 5',
                        key: 'c5'
                    },
                    {
                        minWidth: 100,
                        title: 'Column 6',
                        key: 'c6'
                    },
                    {
                        minWidth: 100,
                        title: 'Column 7',
                        key: 'c7'
                    },
                    {
                        width: 200,
                        title: 'action',
                        fixed: 'right',
                        render: (h, p) => h('span', 'hello')
                    }
                ],
                data3: [
                    {
                      c1: 'c1 content: testing',
                      c2: 'c2 content: attention please',
                      c3: 'c3 content: ... dudu ...',
                      c4: 'the quick brown fox jumps over the lazy dog.',
                      c5: 'c5 content',
                      c6: 'c6 content',
                      c7: 'c7 content'
                    }
                ],
                columns2: [
                    {
                        title: 'Name',
                        key: 'name',
                        width: 100,
//                        fixed: 'left'
                    },
                    {
                        title: 'Age',
                        key: 'age',
                        width: 100
                    },
                    {
                        title: 'Province',
                        key: 'province',
                        width: 100
                    },
                    {
                        title: 'City',
                        key: 'city',
                        width: 100
                    },
                    {
                        title: 'Address',
                        key: 'address',
                        width: 200
                    },
                    {
                        title: 'Postcode',
                        key: 'zip',
                        width: 100
                    },
                    {
                        title: 'Action',
                        key: 'action',
                        fixed: 'right',
                        width: 120,
                        render: (h, params) => {
                            return h('div', [
                                h('Button', {
                                    props: {
                                        type: 'text',
                                        size: 'small'
                                    }
                                }, 'View'),
                                h('Button', {
                                    props: {
                                        type: 'text',
                                        size: 'small'
                                    }
                                }, 'Edit')
                            ]);
                        }
                    }
                ],
                data4: [
                    {
                        name: 'John Brown',
                        age: 18,
                        address: 'New York No. 1 Lake Park',
                        province: 'America',
                        city: 'New York',
                        zip: 100000
                    },
                    {
                        name: 'Jim Green',
                        age: 24,
                        address: 'Washington, D.C. No. 1 Lake Park',
                        province: 'America',
                        city: 'Washington, D.C.',
                        zip: 100000
                    },
                    {
                        name: 'Joe Black',
                        age: 30,
                        address: 'Sydney No. 1 Lake Park',
                        province: 'Australian',
                        city: 'Sydney',
                        zip: 100000
                    },
                    {
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa No. 2 Lake Park',
                        province: 'Canada',
                        city: 'Ottawa',
                        zip: 100000
                    },
                    {
                        name: 'John Brown',
                        age: 18,
                        address: 'New York No. 1 Lake Park',
                        province: 'America',
                        city: 'New York',
                        zip: 100000
                    },
                    {
                        name: 'Jim Green',
                        age: 24,
                        address: 'Washington, D.C. No. 1 Lake Park',
                        province: 'America',
                        city: 'Washington, D.C.',
                        zip: 100000
                    },
                    {
                        name: 'Joe Black',
                        age: 30,
                        address: 'Sydney No. 1 Lake Park',
                        province: 'Australian',
                        city: 'Sydney',
                        zip: 100000
                    },
                    {
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa No. 2 Lake Park',
                        province: 'Canada',
                        city: 'Ottawa',
                        zip: 100000
                    }
                ]
            }
        }
    }
</script>

