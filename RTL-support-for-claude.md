.font-claude-response-body,
.standard-markdown p,
.standard-markdown li,
.standard-markdown h1,
.standard-markdown h2,
.standard-markdown h3,
.standard-markdown h4 {
  unicode-bidi: plaintext !important;
  text-align: start !important;
}

.standard-markdown ul,
.standard-markdown ol {
  unicode-bidi: plaintext !important;
}

.standard-markdown pre,
.standard-markdown code,
.font-claude-response pre,
.font-claude-response code {
  unicode-bidi: normal !important;
  direction: ltr !important;
  text-align: left !important;
}


.standard-markdown ul,
.standard-markdown ol,
.font-claude-response ul,
.font-claude-response ol {
  direction: rtl !important;
  unicode-bidi: plaintext !important;
}

.standard-markdown :not(pre) > code {
  unicode-bidi: isolate !important;
  direction: ltr !important;
}


.standard-markdown table {
  direction: rtl !important;
}


.standard-markdown th,
.standard-markdown td {
  unicode-bidi: isolate !important;
  text-align: right !important;
}

.standard-markdown table.table-ltr {
  direction: ltr !important;
}


.standard-markdown li,
.font-claude-response-body li {
  unicode-bidi: plaintext;
  direction: rtl;
  text-align: right;
}


.standard-markdown li strong:first-child,
.font-claude-response-body li strong:first-child {
  unicode-bidi: isolate;
  display: inline-block;
}


span.truncate.font-base {
  unicode-bidi: plaintext;
}


.font-base {
  unicode-bidi: plaintext;
}
