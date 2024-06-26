###VIETNAMESE translation below


<a href = "https://drive.google.com/drive/folders/1nIHVzezOzOM2ZuvnHWou7NtjhrcpCZzi?usp=drive_link">
Click for demo video</a>


##


###ENGLISH

This is a simple audio application program (i.e. an app) called MyAudio implemented in Java.

The MyAudio app stores and manages audio content of various types (e.g. Songs, Audio Books, Podcasts) in a library. Audio content can be downloaded from a simulated online store.
The audio content in the library can be played (i.e. in this app, playing a song means printing its lyrics). 
Playlists can be created from library content. A playlist can store songs or even a mixture of different types of audio content

#Every part of this project is a sample code which shows how to do the following:

1.	Library: this class contains the bulk of the logic for the app. It maintains an array list of songs, an array list of audiobooks, an array list of podcasts and an array list of playlists. 

2.	MyAudioUI: This class has the main() method and the user interface (UI). Some UI skeleton code has been provided for you with some comments. In a while loop, a scanner reads a line of input from the user. The input lines contain words (Strings) which represent actions (e.g. songs, store, download etc). Some actions require parameters to be input by the user. The parameters may be strings or an integer. 

3.	AudioContent: class AudioContent is a general superclass containing several instance variables (see the skeleton code) that model audio content. This class can be extended to model more specific types of audio content (e.g. song, podcast, audiobook). It has instance variables: title (String), year (int), id (String), type (String), audioFile (String), length (int). For example a title might be “Yesterday”. The ID (a string) is generated by the system (e.g. “913”). 

4.	AudioContentStore: class AudioContentStore simulates an online store. The MyAudio app can download content (e.g. a song, an audiobook) from this store to your library. When the user types the action STORE then a method is called to list the store contents. The contents are numbered (1, 2, 3 etc). Each content has a type (Song, AudioBook, Podcast). The user can type the DOWNLOAD action and then specify the number of the content they want stored in their library
   
5.	Song: class Song is a subclass of Audio Content (i.e. a song is a type of audio content). In addition to the AudioContent information, a song has fields to store the artist name, the composer name, the genre and the lyrics.
   
6.	AudioBook: This class is also a subclass of AudioContent that contains extra information. An AudioBook contains the book’s author and AudioBook’s narrator. It also contains two array lists of Strings: one that contains the chapter titles and one that contains the chapter contents. The class has a method to select a specific chapter to play. 

7.	Playlist: class Playlist stores a list of audio content (e.g. songs or audiobooks or podcasts or even a mixture of these). A Playlist is given a title (e.g. “Workout” “Dinner Music” “Dance Mix”). There are a series of user actions to make a playlist, add content to a playlist etc. All the content can be played (i.e. playAll()) or a specific audio content can be played (e.g. song 5)

###=================================================================================

##VIETNAMESE

Đây là một chương trình ứng dụng âm thanh đơn giản (tức là một ứng dụng) có tên MyAudio được triển khai bằng Java.

Ứng dụng MyAudio lưu trữ và quản lý nhiều loại nội dung âm thanh (ví dụ: Bài hát, Sách nói, Podcast) trong thư viện. Nội dung âm thanh có thể được tải xuống từ một cửa hàng trực tuyến mô phỏng.
Có thể phát nội dung âm thanh trong thư viện (tức là trong ứng dụng này, phát một bài hát có nghĩa là in lời bài hát).
Danh sách phát có thể được tạo từ nội dung thư viện. Danh sách phát có thể lưu trữ các bài hát hoặc thậm chí là hỗn hợp các loại nội dung âm thanh khác nhau

#Mỗi phần của dự án này là một mã mẫu cho biết cách thực hiện những điều sau:

1. Thư viện: lớp này chứa phần lớn logic cho ứng dụng. Nó duy trì một danh sách các bài hát, một danh sách các sách nói, một danh sách các podcast và một danh sách các danh sách phát.

2. MyAudioUI: Lớp này có phương thức main() và giao diện người dùng (UI). Một số mã khung giao diện người dùng đã được cung cấp cho bạn kèm theo một số nhận xét. Trong vòng lặp while, máy quét sẽ đọc dòng đầu vào từ người dùng. Các dòng đầu vào chứa các từ (Chuỗi) đại diện cho các hành động (ví dụ: bài hát, cửa hàng, tải xuống, v.v.). Một số hành động yêu cầu người dùng phải nhập tham số. Các tham số có thể là chuỗi hoặc số nguyên.

3. AudioContent: lớp AudioContent là một siêu lớp chung chứa một số biến thể hiện (xem mã khung) mô hình hóa nội dung âm thanh. Lớp này có thể được mở rộng để mô hình hóa các loại nội dung âm thanh cụ thể hơn (ví dụ: bài hát, podcast, sách nói). Nó có các biến thể hiện: tiêu đề (Chuỗi), năm (int), id (Chuỗi), loại (Chuỗi), audioFile (Chuỗi), độ dài (int). Ví dụ: tiêu đề có thể là “Hôm qua”. ID (một chuỗi) được tạo bởi hệ thống (ví dụ: “913”).

4. AudioContentStore: lớp AudioContentStore mô phỏng một cửa hàng trực tuyến. Ứng dụng MyAudio có thể tải nội dung (ví dụ: một bài hát, sách nói) từ cửa hàng này về thư viện của bạn. Khi người dùng gõ hành động STORE thì một phương thức sẽ được gọi để liệt kê nội dung của cửa hàng. Nội dung được đánh số (1, 2, 3, v.v.). Mỗi nội dung có một loại (Bài hát, AudioBook, Podcast). Người dùng có thể nhập hành động TẢI XUỐNG rồi chỉ định số lượng nội dung họ muốn lưu trữ trong thư viện của mình
   
5. Bài hát: lớp Bài hát là một lớp con của Nội dung âm thanh (tức là bài hát là một loại nội dung âm thanh). Ngoài thông tin AudioContent, một bài hát còn có các trường để lưu trữ tên nghệ sĩ, tên nhà soạn nhạc, thể loại và lời bài hát.
   
6. AudioBook: Lớp này cũng là một lớp con của AudioContent chứa thông tin bổ sung. AudioBook chứa tác giả của cuốn sách và người kể chuyện của AudioBook. Nó cũng chứa hai danh sách mảng Chuỗi: một danh sách chứa tiêu đề chương và một danh sách chứa nội dung chương. Lớp có phương pháp chọn một chương cụ thể để chơi.

7. Danh sách phát: lớp Danh sách phát lưu trữ danh sách nội dung âm thanh (ví dụ: bài hát, sách nói hoặc podcast hoặc thậm chí là hỗn hợp của những nội dung này). Danh sách phát được đặt tiêu đề (ví dụ: “Tập luyện” “Âm nhạc bữa tối” “Dance Mix”). Có một loạt hành động của người dùng để tạo danh sách phát, thêm nội dung vào danh sách phát, v.v. Có thể phát tất cả nội dung (tức là playAll()) hoặc có thể phát một nội dung âm thanh cụ thể (ví dụ: bài hát 5)
