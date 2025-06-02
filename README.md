# Fonctions

## Fonctions partie 1 :

`size_t ft_strlen(const char *s)` -> Calcule la longueur d'une chaîne de caractères. <br>
size_t ft_strlcat(char *dst, const char *src, size_t dstsize) -> Concatène deux chaînes de caractères en limitant la taille du résultat.<br>
size_t ft_strlcpy(char *dst, const char *src, size_t dstsize) -> Copie une chaîne de caractères dans une autre en limitant la taille de destination.<br>
void ft_bzero(void *s, size_t n) -> Remplit les premiers octets de la mémoire pointée par `s` avec l'octet nul (valeur 0). <br>
void *ft_memchr(const void *s, int c, size_t n) -> Recherche une valeur dans une zone mémoire.<br>
void *ft_memcpy(void *dst, const void *src, size_t n) -> Copie une zone mémoire source dans une zone mémoire destination. <br>
void *ft_memmove(void *dest, const void *src, size_t len) -> Copie une zone mémoire source dans une zone mémoire destination, même si elles se chevauchent.<br>
void *ft_memset(void *s, int c, size_t n) -> Remplit une zone mémoire avec une valeur donnée. <br>
void *ft_calloc(size_t nmemb, size_t size) -> Alloue et initialise un bloc de mémoire à zéro.<br>
char *ft_strchr(const char *s, int c) -> Recherche la première occurrence d'un caractère dans une chaîne de caractères.<br>
char *ft_strdup(const char *s1) -> Duplique une chaîne de caractères.<br>
char *ft_strrchr(const char *s, int c) -> Recherche la dernière occurrence d'un caractère dans une chaîne de caractères.<br>
char *ft_strnstr(const char *haystack, const char *needle, size_t n) -> Recherche une sous-chaîne dans une chaîne avec une limite de longueur.<br>
int ft_isalpha(int c) -> Vérifie si le caractère passé en argument est une lettre alphabétique. <br>
int ft_atoi(const char *str) -> Convertit une chaîne de caractères en un entier.<br>
int ft_isalnum(int c) -> Vérifie si le caractère passé en argument est un caractère alphanumérique. <br>
int ft_isascii(int c) -> Vérifie si le caractère passé en argument est un caractère ASCII. <br>
int ft_isdigit(int c) -> Vérifie si le caractère passé en argument est un chiffre décimal. <br>
int ft_isprint(int c) -> Vérifie si le caractère passé en argument est un caractère imprimable. <br>
int ft_memcmp(const void *s1, const void *s2, size_t n) -> Compare les n premiers octets de deux zones mémoire.<br>
int ft_toupper(int c) -> Convertit un caractère minuscule en caractère majuscule si c'est une lettre minuscule.<br>
int ft_tolower(int c) -> Convertit un caractère majuscule en caractère minuscule si c'est une lettre majuscule.<br>
int ft_strncmp(const char *s1, const char *s2, size_t n) -> Compare les n premiers caractères de deux chaînes de caractères.<br>

## Fonctions partie 2 :

void ft_putchar_fd(char c, int fd) -> Écrit le caractère c sur la sortie correspondant au descripteur de fichier fd.
void ft_putstr_fd(char *s, int fd) -> Écrit la chaîne de caractères terminée par '\0' (s) sur le descripteur fd, sans ajouter de retour à la ligne à la fin.
void ft_putendl_fd(char *s, int fd) -> Même comportement que ft_putstr_fd, mais ajoute un caractère de nouvelle ligne ('\n') à la fin.
void ft_putnbr_fd(int n, int fd) -> Convertit l’entier n en sa représentation décimale ASCII et l’écrit sur fd. Gère également le signe négatif.
void ft_striteri(char *s, void (*f)(unsigned int, char*)) -> Applique une fonction à chaque caractère d'une chaîne avec son index en argument.
char *ft_strjoin(char const *s1, char const *s2) -> Concatène deux chaînes de caractères.<br>
char *ft_substr(char const *s, unsigned int start, size_t len) -> Extrait une sous-chaîne d'une chaîne de caractères.<br>
char *ft_strtrim(char const *s1, char const *set) -> Supprime les caractères spécifiés en début et en fin d'une chaîne de caractères.<br>
char *ft_strmapi(char const *s, char (*f)(unsigned int, char)) -> Applique une fonction à chaque caractère d'une chaîne avec son index en argument.<br>
char *ft_itoa(int n) -> Convertit un entier en chaîne de caractères.<br>
char **ft_split(char const *s, char c) -> Divise une chaîne de caractères en mots en utilisant un caractère délimiteur.<br>


## Fonctions bonus :

t_list	*ft_lstnew(void *content) -> Crée un nouvel élément de liste avec la donnée passée en argument.
t_list	*ft_lstlast(t_list *lst) ->  Renvoie un pointeur vers le dernier élément de la liste.
t_list	*ft_lstmap(t_list *lst, void *(*f)(void *), void (*del)(void *)) -> Applique la fonction 'f' à chaque élément de la liste, crée une nouvelle liste avec les résultats et retourne un pointeur vers la nouvelle liste. En cas d'échec d'allocation mémoire, libère la nouvelle liste ainsi que son contenu en utilisant 'del' et renvoie NULL.
void	ft_lstadd_front(t_list **lst, t_list *new) -> Ajoute un nouvel élément au début de la liste.<br>
void	ft_lstadd_back(t_list **lst, t_list *new) -> Ajoute un élément à la fin de la liste chaînée.<br>
void	ft_lstdelone(t_list *lst, void (*del)(void *)) -> Supprime un élément de la liste sans supprimer la structure de données qu'il contenait.<br>
void	ft_lstclear(t_list **lst, void (*del)(void *)) -> Supprime et libère la mémoire de tous les éléments de la liste en utilisant une fonction de suppression.<br>
void	ft_lstiter(t_list *lst, void (*f)(void *)) -> Applique la fonction 'f' à chaque 'content' de 'lst'.<br>
int		ft_lstsize(t_list *lst) -> Calcule la taille de la liste en comptant le nombre d'éléments.<br>
