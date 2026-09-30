- Dòng lệnh sai:
    + for (let cupIndex = 1; cupIndex < orderQuantity; cupIndex++)
    điều kiện thực thi vòng lặp sai, theo đơn đặt hàng của khách là 3 ly nhưng trong vòng lặp chỉ chạy đến < orderQuantity tức là chỉ chạy 1, 2 thiếu một đúng phải là <= orderQuantity
    + if (isGoldMember) {
    totalBill = totalBill * 0.9;
    } đặt sai vị trí dẫn đến mỗi lần vòng lặp chạy một lần sẽ giảm giá 10% mỗi lần, để xử lí thì cần chuyển đòng if ra bên ngoài vòng lặp for

- Bảng test case:
    |---|---|---|---|
    |Trường hợp kiểm thử|Dữ liệu đầu vào|Kết quả sai sót|Kết quả mong đợi|
    |---|---|---|---|
    |Trường hợp đúng như đề với code chưa qua chỉnh sửa|orderQuantity = 3,drinkSize = "M", toppingsPerCup = 2, isGoldMember = true| 87210 | 137700|
    |Thay đổi trường hợp isGoldMember = false| orderQuantity = 3,drinkSize = "M", toppingsPerCup = 2, isGoldMember = true| 102000 | 153000|
    |---|---|---|---|