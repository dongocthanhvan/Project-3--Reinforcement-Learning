# UC-Berkeley-CS188_cu-ng-c-
Câu 1: Nhiệm vụ là lặp lại các giá trị liên tiếp giới hạn độ sâu phản ánh phần thưởng tiếp theo bắt đầu với Vo=k, cho Vk và tính giá trị của độ sâu k+1 chot tất cả các trạng thái 
+Sử dụng vòng lặp giá trị được thiết lập cho các lần lặp 
+Khai báo 1 bộ đếm để lưu các giá trị của lần lặp cho mọi trạng thái 
+Nhìn vào state nếu trạng thái là trạng thái kết thúc ,phần thưởng là phần tưởng thoát và không có phần thưởng triết khấu 
 và nếu chưa phải trạng thái kết thúc thì tìm giá trị tốt nhất làm tổng phần thưởng 


Câu 2:Phân tích điểm qua cầu
 Với noise =0 vấn đề trở lên sáng tỏ và tác nhân sẽ luôn kết thúc còn ở trạng thái dự kiến ,nên chính sách tối ưu sẽ vượt qua cầu
 + Vì nó sẽ luôn di chuyển theo hướng tối đa hóa phần thưởng mong đợi 
 
 
Câu 3:Chính sách : Mô tả có 4 trạng thái đường đi có thể kết thúc ở +1 , rủi ro đi qua đá,kết thúc ở 10 với rủi ro đi qua đá , kết thúc ở 10 nếu không đi qua đá
 a.-Vì muốn nhanh chóng di chuyển đến lối toát phần tưởng và độ ổn định 
 +Được giữ lại để cố gắng toát ra càng sớm càng tốt 
 -> nếu khả thi thì trả về "NOT POSSIBLE"
 
 
Câu 4:Q-Learning: 
- hoàn thành các hàm getQvalue , comutevaluFromvalues học bằng cách thử và sai từ các tương tác với môi trường thông qua update(state, action, nextState, reward
+Nhận tất cả các giá trị hành động của trạng thái ,giá trị cho trạng thái cuối là 0
+Giá trị của các trạng thái khác là giá trị tối đá của các giá trị trạng thái 


Câu 5:Tính tham lam của Epsilon
- Đối với epsilon tham lam chọn thời gian epsilon hành động ngẫu nhiên và thời gian 1 epsilon tối ưu 
 Hoàn thành tác nhân Q-learning bằng cách triển khai lựa chọn hành động tham lam epsilon getAction, nghĩa là nó chọn các hành động ngẫu nhiên trong một phần thời gian epsilon và theo cách khác, giá trị Q tốt nhất hiện tại của nó
 
 
Câu 6:Chiếu lại qua cầu 
-Chúng ta sẽ thiết lập answerEpsilon và answerlearningRate
+Nếu không tìm được đường đi tối ưu vì số 50 tập quá nhỏ 
+Nếu không khả thi trả về" NOT POSSIBLE"

Câu 7: Q-Learning và Pacman
Nó có thể nhận thấy sau koảng thời gian pacman sẽ chơi thông minh hơn do số lần chuyên quá nhỏ nên pacman vẫn chưa thắng được
van dung chay vs pacman


Câu 8:Q-Learning gần đúng
-Hoàn thành hàm tối ưu approximateQAgent
+Đối với mỗi tính năng trích xuất cho trạng thái và trọng số tương ứng của hành động--> nên được trích xuất trả về giá trị của 1 trạng thái đó là tổng (f i (s,a)*w i)
--> cũng như phần trước chúng ta có thể thấy là pacman càng chơi càng thông minh với kết quả này chúng ta đều thắng .
 
