英文原文地址：http://ejohn.org/blog/how-javascript-timers-work/
中文地址： http://www.lxway.com/60615592.htm

        function formatDate(devider, date) {
            var date = date || new Date();
            var devider = devider || '-';
            console.log(date.getHours() + devider + date.getMinutes() + devider + date.getSeconds() + devider + date.getMilliseconds());
        }

        var interval = setInterval(function () {
            console.log('interval');
            formatDate('::');
        }, 2000);

        var start = new Date();
        formatDate();
        for(let i=0; i<1; i++) {
            start = new Date();
            while(new Date() - start < 5 * 1000) {

            }
            formatDate();
        }
        
  keys1:  
