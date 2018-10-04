
<script>



    new Vue({
		
	

      
    
     
	

		
            show:true,
            el: '#app',
			
			data: () => ({
				
	
	
	
  }),
 
  
            data: () => ({
				
            pagination: {
                sortBy: 'name'
				
            },
            selected: [],
            headers: [

                { text: 'دکمه ها', value: 'buttons' },
                { text: 'وضعیت', value: 'state' },
                { text: 'تاریخ ارسال', value: 'date' },
                { text: 'عنوان درخواست', value: 'requestTitle' },
                { text: 'ردیف', value: 'rowNumber' }
            ],
            rowNumber: [
                {
                    value: false,
                    buttons: '',
                    state: 'تایید نشده',
                    date: '1379/3/2',
                    requestTitle: 'درخواست لورم اسپیوم',
                    rowNumber: '1'
                },
                {
                    value: false,
                    buttons: 237,
                    state: 'تایید نشده',
                    date: '1379/3/2',
                    requestTitle: 'درخواست لورم اسپیوم',
                    rowNumber: '2'
                },
                {
                    value: false,
                    buttons: 262,
                    state: 'تایید نشده',
                    date: '1379/3/2',
                    requestTitle: 'درخواست لورم اسپیوم',
                    rowNumber: '3'
                },
                {
                    value: false,
                    buttons: 305,
                    state: 'تایید نشده',
                    date: '1379/3/2',
                    requestTitle: 'درخواست لورم اسپیوم',
                    rowNumber: '4'
                },
                {
                    value: false,
                    buttons: 356,
                    state: 'تایید نشده',
                    date: '1379/3/2',
                    requestTitle: 'درخواست لورم اسپیوم',
                    rowNumber: '5'
                },
                {
                    value: false,
                    buttons: 375,
                    state: 'تایید نشده',
                    date: '1379/3/2',
                    requestTitle: 'درخواست لورم اسپیوم',
                    rowNumber: '6'
                },
                {
                    value: false,
                    buttons: 392,
                    state: 'تایید نشده',
                    date: '1379/3/2',
                    requestTitle: 'درخواست لورم اسپیوم',
                    rowNumber: '7'
                },
                {
                    value: false,
                    buttons: 408,
                    state: 'تایید نشده',
                    date: '1379/3/2',
                    requestTitle: 'درخواست لورم اسپیوم',
                    rowNumber: '8'
                },
                {
                    value: false,
                    buttons: 452,
                    state: 'تایید نشده',
                    date: '1379/3/2',
                    requestTitle: 'درخواست لورم اسپیوم',
                    rowNumber: '9'
                },
                {
                    value: false,
                    buttons: 518,
                    state: 'تایید نشده',
                    date: '1379/3/2',
                    requestTitle: 'درخواست لورم اسپیوم',
                    rowNumber: '10'
                }

            ]
        }),

        methods: {
        toggleAll (){
            if (this.selected.length) this.selected = []
            else this.selected = this.desserts.slice()
        },
        changeSort (column){
            if (this.pagination.sortBy === column) {
                this.pagination.descending = !this.pagination.descending
            } else {
                this.pagination.sortBy = column
                this.pagination.descending = false
            }
        },
        next (){
            const active = parseInt(this.active)
            this.active = (active < 2 ? active + 1 : 0)
        },
    }


  
    })
</script>
