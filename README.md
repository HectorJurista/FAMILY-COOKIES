# FAMILY-COOKIES
FAMILY COOKIES IS A PREOJECT EN DATA SCIENCE IN PYTHON TO ELABORATE DESCRIPTION ABOUT CIA
from http.cookies import SimpleCookie

def set_cookie():
    cookie = SimpleCookie()
    cookie["session_id"] = "66LL3CH1"
    cookie["session_id"]["path"] = "/"
    cookie["session_id"]["httponly"] = True  # Protege contra accesos en JavaScript
    print(cookie.output())

def get_cookie(headers):
    cookie = SimpleCookie()
    if "Cookie" in headers:
        cookie.load(headers["Cookie"])
        if "session_id" in cookie:
            return cookie["session_id"].value
    return None

# Ejemplo de uso
if __name__ == "__main__":
    print("Seteando cookie:")
    set_cookie()
    
    headers_example = {"Cookie": "session_id=66LL3CH1"}
    print("Recuperando cookie:")
    print(get_cookie(headers_example))
from http.cookies import SimpleCookie

def set_cookie():
    cookie = SimpleCookie()
    cookie["session_id"] = "66LL3CH1"
    cookie["session_id"]["path"] = "/"
    cookie["session_id"]["httponly"] = True  # Protege contra accesos en JavaScript
    
    cookie["user_id"] = "12345"
    cookie["user_id"]["path"] = "/"
    
    cookie["theme"] = "dark"
    cookie["theme"]["path"] = "/"
    
    print(cookie.output())

def get_cookie(headers):
    cookie = SimpleCookie()
    if "Cookie" in headers:
        cookie.load(headers["Cookie"])
        cookies_dict = {key: cookie[key].value for key in cookie.keys()}
        return cookies_dict
    return None

# Ejemplo de uso
if __name__ == "__main__":
    print("Seteando cookies:")
    set_cookie()
    
    headers_example = {"Cookie": "session_id=66LL3CH1; user_id=12345; theme=dark"}
    print("Recuperando cookies:")
    print(get_cookie(headers_example))
from http.cookies import SimpleCookie

def set_cookie():
    cookie = SimpleCookie()
    cookie["session_id"] = "66LL3CH1"
    cookie["session_id"]["path"] = "/"
    cookie["session_id"]["httponly"] = True  # Protege contra accesos en JavaScript
    
    cookie["user_id"] = "12345"
    cookie["user_id"]["path"] = "/"
    
    cookie["theme"] = "dark"
    cookie["theme"]["path"] = "/"
    
    cookie["language"] = "es"
    cookie["language"]["path"] = "/"
    
    cookie["token"] = "abcdef123456"
    cookie["token"]["path"] = "/"
    cookie["token"]["secure"] = True  # Solo se envía a través de HTTPS
    
    cookie["preferences"] = "notifications:on"
    cookie["preferences"]["path"] = "/"
    
    print(cookie.output())

def get_cookie(headers):
    cookie = SimpleCookie()
    if "Cookie" in headers:
        cookie.load(headers["Cookie"])
        cookies_dict = {key: cookie[key].value for key in cookie.keys()}
        return cookies_dict
    return None

# Ejemplo de uso
if __name__ == "__main__":
    print("Seteando cookies:")
    set_cookie()
    
    headers_example = {"Cookie": "session_id=66LL3CH1; user_id=12345; theme=dark; language=es; token=abcdef123456; preferences=notifications:on"}
    print("Recuperando cookies:")
    print(get_cookie(headers_example))
from http.cookies import SimpleCookie

def set_cookie():
    cookie = SimpleCookie()
    cookie["session_id"] = "66LL3CH1"
    cookie["session_id"]["path"] = "/"
    cookie["session_id"]["httponly"] = True  # Protege contra accesos en JavaScript
    
    cookie["user_id"] = "12345"
    cookie["user_id"]["path"] = "/"
    
    cookie["theme"] = "dark"
    cookie["theme"]["path"] = "/"
    
    cookie["language"] = "es"
    cookie["language"]["path"] = "/"
    
    cookie["token"] = "abcdef123456"
    cookie["token"]["path"] = "/"
    cookie["token"]["secure"] = True  # Solo se envía a través de HTTPS
    
    cookie["preferences"] = "notifications:on"
    cookie["preferences"]["path"] = "/"
    
    cookie["last_login"] = "2025-03-07T12:00:00Z"
    cookie["last_login"]["path"] = "/"
    
    cookie["session_timeout"] = "3600"
    cookie["session_timeout"]["path"] = "/"
    
    print(cookie.output())

def get_cookie(headers):
    cookie = SimpleCookie()
    if "Cookie" in headers:
        cookie.load(headers["Cookie"])
        cookies_dict = {key: cookie[key].value for key in cookie.keys()}
        return cookies_dict
    return None

def delete_cookie():
    cookie = SimpleCookie()
    cookie["session_id"] = ""
    cookie["session_id"]["path"] = "/"
    cookie["session_id"]["expires"] = "Thu, 01 Jan 1970 00:00:00 GMT"
    print(cookie.output())

# Ejemplo de uso
if __name__ == "__main__":
    print("Seteando cookies:")
    set_cookie()
    
    headers_example = {"Cookie": "session_id=66LL3CH1; user_id=12345; theme=dark; language=es; token=abcdef123456; preferences=notifications:on; last_login=2025-03-07T12:00:00Z; session_timeout=3600"}
    print("Recuperando cookies:")
    print(get_cookie(headers_example))
    
    print("Eliminando cookie de sesión:")
    delete_cookie()
    from http.cookies import SimpleCookie

def set_cookie():
    cookie = SimpleCookie()
    cookie["session_id"] = "66LL3CH1"
    cookie["session_id"]["path"] = "/"
    cookie["session_id"]["httponly"] = True  # Protege contra accesos en JavaScript
    
    cookie["user_id"] = "12345"
    cookie["user_id"]["path"] = "/"
    
    cookie["theme"] = "dark"
    cookie["theme"]["path"] = "/"
    
    cookie["language"] = "es"
    cookie["language"]["path"] = "/"
    
    cookie["token"] = "abcdef123456"
    cookie["token"]["path"] = "/"
    cookie["token"]["secure"] = True  # Solo se envía a través de HTTPS
    
    cookie["preferences"] = "notifications:on"
    cookie["preferences"]["path"] = "/"
    
    cookie["last_login"] = "2025-03-07T12:00:00Z"
    cookie["last_login"]["path"] = "/"
    
    cookie["session_timeout"] = "3600"
    cookie["session_timeout"]["path"] = "/"
    
    cookie["device"] = "mobile"
    cookie["device"]["path"] = "/"
    
    cookie["location"] = "Colombia"
    cookie["location"]["path"] = "/"
    
    cookie["security_level"] = "high"
    cookie["security_level"]["path"] = "/"
    
    cookie["cart_items"] = "5"
    cookie["cart_items"]["path"] = "/"
    
    print(cookie.output())

def get_cookie(headers):
    cookie = SimpleCookie()
    if "Cookie" in headers:
        cookie.load(headers["Cookie"])
        cookies_dict = {key: cookie[key].value for key in cookie.keys()}
        return cookies_dict
    return None

def delete_cookie():
    cookie = SimpleCookie()
    cookie["session_id"] = ""
    cookie["session_id"]["path"] = "/"
    cookie["session_id"]["expires"] = "Thu, 01 Jan 1970 00:00:00 GMT"
    
    cookie["token"] = ""
    cookie["token"]["path"] = "/"
    cookie["token"]["expires"] = "Thu, 01 Jan 1970 00:00:00 GMT"
    
    print(cookie.output())

def update_cookie(headers, key, value):
    cookie = SimpleCookie()
    if "Cookie" in headers:
        cookie.load(headers["Cookie"])
    cookie[key] = value
    cookie[key]["path"] = "/"
    print(cookie.output())

# Ejemplo de uso
if __name__ == "__main__":
    print("Seteando cookies:")
    set_cookie()
    
    headers_example = {"Cookie": "session_id=66LL3CH1; user_id=12345; theme=dark; language=es; token=abcdef123456; preferences=notifications:on; last_login=2025-03-07T12:00:00Z; session_timeout=3600; device=mobile; location=Colombia; security_level=high; cart_items=5"}
    print("Recuperando cookies:")
    print(get_cookie(headers_example))
    
    print("Actualizando cookie de seguridad:")
    update_cookie(headers_example, "security_level", "medium")
    
    print("Eliminando cookies de sesión y token:")
    delete_cookie()
    from http.cookies import SimpleCookie

def set_cookie():
    cookie = SimpleCookie()
    cookie["session_id"] = "66LL3CH1"
    cookie["session_id"]["path"] = "/"
    cookie["session_id"]["httponly"] = True  # Protege contra accesos en JavaScript
    
    cookie["user_id"] = "12345"
    cookie["user_id"]["path"] = "/"
    
    cookie["theme"] = "dark"
    cookie["theme"]["path"] = "/"
    
    cookie["language"] = "es"
    cookie["language"]["path"] = "/"
    
    cookie["token"] = "abcdef123456"
    cookie["token"]["path"] = "/"
    cookie["token"]["secure"] = True  # Solo se envía a través de HTTPS
    
    cookie["preferences"] = "notifications:on"
    cookie["preferences"]["path"] = "/"
    
    cookie["last_login"] = "2025-03-07T12:00:00Z"
    cookie["last_login"]["path"] = "/"
    
    cookie["session_timeout"] = "3600"
    cookie["session_timeout"]["path"] = "/"
    
    cookie["device"] = "mobile"
    cookie["device"]["path"] = "/"
    
    cookie["location"] = "Colombia"
    cookie["location"]["path"] = "/"
    
    cookie["security_level"] = "high"
    cookie["security_level"]["path"] = "/"
    
    cookie["cart_items"] = "5"
    cookie["cart_items"]["path"] = "/"
    
    cookie["exam_mode"] = "enabled"
    cookie["exam_mode"]["path"] = "/"
    
    cookie["exam_attempts"] = "2"
    cookie["exam_attempts"]["path"] = "/"
    
    print(cookie.output())

def get_cookie(headers):
    cookie = SimpleCookie()
    if "Cookie" in headers:
        cookie.load(headers["Cookie"])
        cookies_dict = {key: cookie[key].value for key in cookie.keys()}
        return cookies_dict
    return None

def delete_cookie():
    cookie = SimpleCookie()
    cookie["session_id"] = ""
    cookie["session_id"]["path"] = "/"
    cookie["session_id"]["expires"] = "Thu, 01 Jan 1970 00:00:00 GMT"
    
    cookie["token"] = ""
    cookie["token"]["path"] = "/"
    cookie["token"]["expires"] = "Thu, 01 Jan 1970 00:00:00 GMT"
    
    print(cookie.output())

def update_cookie(headers, key, value):
    cookie = SimpleCookie()
    if "Cookie" in headers:
        cookie.load(headers["Cookie"])
    cookie[key] = value
    cookie[key]["path"] = "/"
    print(cookie.output())

def examine_cookies(headers):
    print("Examinando cookies recibidas:")
    cookies = get_cookie(headers)
    if cookies:
        for key, value in cookies.items():
            print(f"{key}: {value}")
    else:
        print("No se encontraron cookies.")

# Ejemplo de uso
if __name__ == "__main__":
    print("Seteando cookies:")
    set_cookie()
    
    headers_example = {"Cookie": "session_id=66LL3CH1; user_id=12345; theme=dark; language=es; token=abcdef123456; preferences=notifications:on; last_login=2025-03-07T12:00:00Z; session_timeout=3600; device=mobile; location=Colombia; security_level=high; cart_items=5; exam_mode=enabled; exam_attempts=2"}
    print("Recuperando cookies:")
    print(get_cookie(headers_example))
    
    print("Examinando cookies:")
    examine_cookies(headers_example)
    
    print("Actualizando cookie de seguridad:")
    update_cookie(headers_example, "security_level", "medium")
    
    print("Eliminando cookies de sesión y token:")
    delete_cookie()
from http.cookies import SimpleCookie

def set_cookie():
    cookie = SimpleCookie()
    cookie["session_id"] = "66LL3CH1"
    cookie["session_id"]["path"] = "/"
    cookie["session_id"]["httponly"] = True  # Protege contra accesos en JavaScript
    
    cookie["user_id"] = "12345"
    cookie["user_id"]["path"] = "/"
    
    cookie["theme"] = "dark"
    cookie["theme"]["path"] = "/"
    
    cookie["language"] = "es"
    cookie["language"]["path"] = "/"
    
    cookie["token"] = "abcdef123456"
    cookie["token"]["path"] = "/"
    cookie["token"]["secure"] = True  # Solo se envía a través de HTTPS
    
    cookie["preferences"] = "notifications:on"
    cookie["preferences"]["path"] = "/"
    
    cookie["last_login"] = "2025-03-07T12:00:00Z"
    cookie["last_login"]["path"] = "/"
    
    cookie["session_timeout"] = "3600"
    cookie["session_timeout"]["path"] = "/"
    
    cookie["device"] = "mobile"
    cookie["device"]["path"] = "/"
    
    cookie["location"] = "Colombia"
    cookie["location"]["path"] = "/"
    
    cookie["security_level"] = "high"
    cookie["security_level"]["path"] = "/"
    
    cookie["cart_items"] = "5"
    cookie["cart_items"]["path"] = "/"
    
    cookie["exam_mode"] = "enabled"
    cookie["exam_mode"]["path"] = "/"
    
    cookie["exam_attempts"] = "2"
    cookie["exam_attempts"]["path"] = "/"
    
    cookie["even_numbers"] = "2,4,6,8,10"
    cookie["even_numbers"]["path"] = "/"
    
    print(cookie.output())

def get_cookie(headers):
    cookie = SimpleCookie()
    if "Cookie" in headers:
        cookie.load(headers["Cookie"])
        cookies_dict = {key: cookie[key].value for key in cookie.keys()}
        return cookies_dict
    return None

def delete_cookie():
    cookie = SimpleCookie()
    cookie["session_id"] = ""
    cookie["session_id"]["path"] = "/"
    cookie["session_id"]["expires"] = "Thu, 01 Jan 1970 00:00:00 GMT"
    
    cookie["token"] = ""
    cookie["token"]["path"] = "/"
    cookie["token"]["expires"] = "Thu, 01 Jan 1970 00:00:00 GMT"
    
    print(cookie.output())

def update_cookie(headers, key, value):
    cookie = SimpleCookie()
    if "Cookie" in headers:
        cookie.load(headers["Cookie"])
    cookie[key] = value
    cookie[key]["path"] = "/"
    print(cookie.output())

def examine_cookies(headers):
    print("Examinando cookies recibidas:")
    cookies = get_cookie(headers)
    if cookies:
        for key, value in cookies.items():
            print(f"{key}: {value}")
    else:
        print("No se encontraron cookies.")

# Ejemplo de uso
if __name__ == "__main__":
    print("Seteando cookies:")
    set_cookie()
    
    headers_example = {"Cookie": "session_id=66LL3CH1; user_id=12345; theme=dark; language=es; token=abcdef123456; preferences=notifications:on; last_login=2025-03-07T12:00:00Z; session_timeout=3600; device=mobile; location=Colombia; security_level=high; cart_items=5; exam_mode=enabled; exam_attempts=2; even_numbers=2,4,6,8,10"}
    print("Recuperando cookies:")
    print(get_cookie(headers_example))
    
    print("Examinando cookies:")
    examine_cookies(headers_example)
    
    print("Actualizando cookie de seguridad:")
    update_cookie(headers_example, "security_level", "medium")
    
    print("Eliminando cookies de sesión y token:")
    delete_cookie()
