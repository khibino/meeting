
md_format = \
        markdown+pandoc_title_block+pipe_tables+table_captions+escaped_line_breaks

slide_opts = \
        --standalone --self-contained --slide-level=1

targets = \
	debian-packaging-s5n.html

%-s5n.html: %.txt
	pandoc -f $(md_format) -t s5 $(slide_opts) -o $@ $<

all: $(targets)

clean:
	$(RM) $(targets)
