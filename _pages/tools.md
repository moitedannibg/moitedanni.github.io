---
title: "Инструменти"
permalink: "/tools.html"
---

<div class="container">
    <div class="row gap-y listrecent listrecent listauthor">
    {% for tool in site.tools %}
        <div class="col-lg-6 mb-4">
            <div class="p-4 border rounded">
            <div class="row">
            <div class="col-md-3 mb-4 mb-md-0"><img alt="{{ tool[1].name }}" src="{{ tool[1].avatar }}" class="rounded-circle" height="80" width="80"></div>
            <div class="col-md-9">
            <a href="{{ tool[1].site }}">
            <h4 class="text-dark mb-0"> {{ tool[1].name }} </h4>
            <!-- <small class="d-inline-block mt-1 mb-3 font-weight-normal">(Повече)</small> -->
            <div class="excerpt">{{ tool[1].description }}</div>
            </a>
            <div class="icon-block mt-3 d-flex justify-content-between">  
            <div>
            <a target="_blank" href="{{ tool[1].site }}"><i class="fa fa-globe text-muted" aria-hidden="true"></i></a> &nbsp;
            </div>
            </div>
            </div>
            </div>
            </div>
        </div>
    {% endfor %}
    </div>
</div>