# Hàm lọc từ đệm
def remove_stopwords(question):
    words = question.split()
    filtered_words = [word for word in words if word.lower() not in stopwords_vi]
    return " ".join(filtered_words)

#từ đệm thường xài
stopwords_vi = [
    "a", "ai", "anh", "chị", "em", "anh ấy", "bà", "bạn", "bên", "bằng", "biết", "bị", "bởi", "bất", "cả", 
    "cái", "các", "cần", "càng", "chỉ", "chiếc", "cho", "chứ", "chưa", "chuyện", "có", "còn", "có thể", 
    "cứ", "của", "cùng", "cũng", "cách", "chính", "do", "dưới", "gì", "hay", "hơn", "hết", "hoặc", 
    "i", "khi", "không", "là", "làm", "lại", "lên", "lúc", "làm sao", "mà", "mình", 
]
