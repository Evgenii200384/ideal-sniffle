function qwe(str) {
    var res = [0,0,0];
    str.replace(
        /(php)|(javascript)|(java\b|python|c\+\+)/gi,
        function(s, php, js, etc) {
            php ? res[0]++ : js ? res[1]++ : res[2]++
        });
    pro = res[0]>res[1] && res[0]>res[2] ? 'PHP' : res[1]>res[2] ? 'JavaScript' : 'C++, Java or Python';
    return "You are "+ pro +" programmer.";
}

console.log(
    qwe(
// You are C++, Java or Python programmer.
Поделиться
Улучшить ответ
Отслеживать
ответ дан 27 июл 2024 в 00:00# test
